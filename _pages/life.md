---
layout: page
title: Life
permalink: /life/
description: Beyond the lab
nav: true
nav_order: 6
---

Outside the lab, I enjoy running, hiking and traveling.

<div class="qy-gallery">
{% assign photos = site.data.life_photos | sort: "date" | reverse %}
{% for p in photos %}
  <figure>
    <img src="{{ '/assets/img/' | append: p.file | relative_url }}" alt="{{ p.alt }}" loading="lazy">
    <figcaption>{{ p.caption }} · {{ p.date | date: "%b %Y" }}</figcaption>
  </figure>
{% endfor %}
</div>


{% if site.categories.life %}
<h2>Updates</h2>
<ul>
{% for post in site.categories.life %}
  <li>{{ post.date | date: '%b %d, %Y' }} · <a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
{% endif %}
