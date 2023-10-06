---
layout: default
title: Food
---
{% assign sorted_photos = site.photo_gallery | sort: "weight" %}
<ul class="photo-gallery">
  {% for image in sorted_photos %}
    <a href="{{ image.recipe_url }}">
       <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
    </a>
  {% endfor %}
</ul>