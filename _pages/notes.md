---
layout: default
permalink: /notes/
title: notes
description: Living notes on textbooks and courses.
nav: true
nav_order: 3
---

<div class="post">

  <ul class="post-list">

    {% assign notelist = site.notes | sort: "date" | reverse %}
    {% for note in notelist %}

    {% assign read_time = note.content | number_of_words | divided_by: 180 | plus: 1 %}
    {% assign year = note.date | date: "%Y" %}
    {% assign tags = note.tags | join: "" %}

    <li>
      <h3>
        <a class="post-title" href="{{ note.url | relative_url }}">{{ note.title }}</a>
      </h3>
      <p class="post-meta">
        {{ read_time }} min read &nbsp; &middot; &nbsp;
        {{ note.date | date: '%B %d, %Y' }}
      </p>
      <p class="post-tags">
        <a href="{{ year | prepend: '/notes/' | relative_url }}">
          <i class="fa-solid fa-calendar fa-sm"></i> {{ year }} </a>

        {% if tags != "" %}
        &nbsp; &middot; &nbsp;
          {% for tag in note.tags %}
          <a href="{{ tag | slugify | prepend: '/notes/tag/' | relative_url }}">
            <i class="fa-solid fa-hashtag fa-sm"></i> {{ tag }}</a>
            {% unless forloop.last %}
              &nbsp;
            {% endunless %}
            {% endfor %}
        {% endif %}
      </p>
    </li>

    {% endfor %}

  </ul>

</div>
