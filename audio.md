---
layout: page
title: Audio
permalink: /audio/
---

<h2 class='page-title'>All Audio</h2>

{% assign exhibits = site.pages | where: 'layout','audio' %}
<ul>
  {% for exhibit in exhibits %}
    <li>
      <a href='{{ exhibit.url | absolute_url }}'>
        {{ site.data.data.objects[exhibit.objects_id].Item_Description.title | escape }}
      </a>
    </li>
  {% endfor %}
</ul>