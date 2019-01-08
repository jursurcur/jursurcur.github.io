---
title: "Deliverables"
layout: page
date: 2019-01-01 01:10
tag:
- design
projects: true
hidden: true # don't count this post in blog pagination
description: "meh"
category: project
author: Jessica Lee
---

{% assign sorted_gallery = site.photo_gallery2 | sort: 'weight' %}
<ul class="photo-gallery" style="list-style: none; padding: 0;">
  {% for image in sorted_gallery %}
    <li style = "list-style: none; padding: 0; display: inline-block; width: 32%;">
      <a href="{{ image.link }}">
        <img src="{{ image.image_path }}" alt="{{ image.title }}" style = "width: 100%;">
      </a>
    </li>
  {% endfor %}
</ul>