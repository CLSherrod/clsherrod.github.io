---
title: "Essays"
tagline: "Read essays by Christopher Sherrod."
layout: archive
permalink: /essays/
description: "Browse essays by Christopher Sherrod on living a fulfilling life, meaningful work, creativity, and lifestyle."
excerpt: "A collection of essays by Christopher Sherrod."
preview: "Browse all essays."
breadcrumbs: true
published: false
toc: false
toc_sticky: false
robots: "index,follow"
---

{% assign essay_posts = site.posts | sort: "date" | reverse %}

<div class="entries-list">
  {% for post in essay_posts %}
    {% if post.post_type == "essay" or post.post_type == nil %}
      {% include archive-single.html type="list" %}
    {% endif %}
  {% endfor %}
</div>
