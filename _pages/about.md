---
layout: about
title: about
permalink: /

profile:
  align: right
  image: profile_pic.png
  image_circular: true # crops the image to make it circular

selected_papers: false # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  /* Re-size profile pic on desktop and mobile */
  .profile img {
    width: 100%;
    height: auto;
    display: block;
    margin: 0 auto;
  }

  @media (max-width: 768px) {
    .profile img {
      width: 80%;
    }
  }
</style>

I work as a graduate data scientist in economic consulting (views my own). Prior to this, I completed the MSc in Statistical Science at Oxford.

Currently, I am interested in world models, especially how to scale pretraining on passive data and how useful the resulting representations are for control. Beyond this, I enjoy learning about neuroscience, AI safety, and statistical learning theory.

My aim with this blog is to record and explain various concepts that I encounter in machine learning research, with more emphasis on intuition than rigour. I hope that it will be useful to others exploring related ideas.
