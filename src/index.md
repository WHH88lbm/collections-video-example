---
title: Home
layout: base.njk
tags: navItem
---

<ul>
  {%- for post in collections.post %}
  <li>
  <a href="{{ post.url }}">
  {{ post.data.title }}
  </a>
  </li>
  {%- endfor %}
</ul