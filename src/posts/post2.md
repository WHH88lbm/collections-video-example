---
title: Post 2
layout: post.njk
tags: [post, trees, breeze, rivers, sun]
author: Author 2
---

This is an example post. The second one.

Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aspernatur voluptatum voluptates sint dignissimos dolor ratione officia aliquid. Dolore odit officia ratione a cupiditate quas cum assumenda error? Voluptatem, laborum possimus!

Lorem ipsum dolor sit amet consectetur adipisicing elit. Temporibus ea nobis quas? Voluptatibus rem dolor et quidem sunt nesciunt corporis numquam accusamus, quod beatae laboriosam aliquam vel dolores vero maiores.
<p>Posts by Author 2</p>
<ul role="list">
{% for post in collections.post %}
{% if post.data.author === "Author 2" %}
  <li>
    <a href="{{ post.url }}">
        {{ post.data.title }} by {{author}}
    </a>
  </li>
{% endif %}
{%- endfor %}
</ul>