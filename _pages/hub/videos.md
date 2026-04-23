---
title: "Videos"
tagline: "Watch video posts by Christopher Sherrod."
layout: archive
permalink: /videos/
description: "Browse video posts by Christopher Sherrod, including updates, reflections, and practical guidance."
excerpt: "A collection of video posts by Christopher Sherrod."
preview: "Browse all video posts."
breadcrumbs: true

header:
  overlay_image: /assets/images/headers/blog-header.webp
  overlay_filter: 0.1
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"

published: true

robots: "index,follow"
---

{% assign video_posts = site.posts | where: "post_type", "video" | sort: "date" | reverse %}

{% if video_posts.size > 0 %}
  {% for post in video_posts %}
    {% include archive-single.html type="list" %}
  {% endfor %}
{% else %}
  <p>No video posts yet.</p>
{% endif %}