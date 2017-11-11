---
layout: page
title: Blog
permalink: /blog/
---

<h1 class="major">Posts</h1>
<ul class="alt">
  {% for post in site.posts %}
    {% assign date_format = site.minima.date_format | default: "%b %-d, %Y" %}
    <li>
      <h1><a href="{{ post.url | relative_url }}">{{ post.title | escape }}</a></h1>
      <h4>{{ post.date | date: date_format }}</h4>
    </li>
  {% endfor %}
</ul>
<p>subscribe <a href="{{ "/feed.xml" | relative_url }}">via RSS</a></p>
