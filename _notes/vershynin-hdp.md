---
layout: post
title: "High-Dimensional Probability (Vershynin)"
date: 2026-07-04
# description: test
tags: statistical-learning combinatorial-geometry
related_posts: false
chart:
  echarts: true
---

<style>
  .echarts {
    height: 500px;
  }
</style>

Vershynin, R. (2026). _High-dimensional probability: An introduction with applications in data science_ (2nd ed.). Cambridge University Press. [https://www.math.uci.edu/~rvershyn/papers/HDP-book/HDP-2.pdf](https://www.math.uci.edu/~rvershyn/papers/HDP-book/HDP-2.pdf)

```echarts
{
  "series": [
    {
      "type": "graph",
      "layout": "force",
      "roam": true,
      "zoom": 0.30,
      "scaleLimit": { "min": 0.2, "max": 3 },
      "draggable": true,
      "symbolSize": 16,
      "itemStyle": {
        "color": "#a6a6a6"
      },
      "label": {
        "show": true,
        "position": "bottom",
        "width": 120,
        "overflow": "break"
      },
      "labelLayout": { "moveOverlap": "shiftY" },
      "edgeSymbol": ["none", "arrow"],
      "force": {
        "repulsion": 2000,
        "edgeLength": 300,
        "gravity": 0.02
      },
      "emphasis": {
        "focus": "adjacency",
        "lineStyle": { "opacity": 1, "width": 2.5 }
      },
      "data": [
        { "name": "Caratheodory theorem" },
        { "name": "Approximate Caratheodory theorem" },
        { "name": "Empirical method (of Maurey)" },
        { "name": "Covering polytopes by balls" },
        { "name": "Volume of a polytope" },
        { "name": "High-degree polytopes have small volume" }
      ],
      "links": [
        { "source": "Approximate Caratheodory theorem", "target": "Caratheodory theorem" },
        { "source": "Approximate Caratheodory theorem", "target": "Empirical method (of Maurey)" },
        { "source": "Covering polytopes by balls", "target": "Approximate Caratheodory theorem" },
        { "source": "Volume of a polytope", "target": "Covering polytopes by balls" },
        { "source": "High-degree polytopes have small volume", "target": "Volume of a polytope" }
      ]
    }
  ]
}
```

*TBC...*
