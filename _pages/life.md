---
layout: page
title: life
permalink: /life/
description: Beyond the lab
nav: true
nav_order: 6
---

Outside the lab, I enjoy running, hiking and traveling.

<div class="qy-gallery">
  <figure>
    <img src="{{ '/assets/img/life_mountain.jpg' | relative_url }}" alt="Hiking in the mountains" loading="lazy">
    <figcaption>Hiking</figcaption>
  </figure>
  <figure>
    <img src="{{ '/assets/img/autumn_road.jpg' | relative_url }}" alt="A forest road in autumn" loading="lazy">
    <figcaption>Autumn colors</figcaption>
  </figure>
</div>

{% if site.categories.life %}
<h2>Updates</h2>
<ul>
{% for post in site.categories.life %}
  <li>{{ post.date | date: '%b %d, %Y' }} · <a href="{{ post.url | relative_url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>
{% endif %}
