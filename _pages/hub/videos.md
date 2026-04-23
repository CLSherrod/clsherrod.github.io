---
title: "Videos"
tagline: "Watch video posts by Christopher Sherrod."
layout: archive
permalink: /videos/
description: "Browse video posts by Christopher Sherrod, including updates, reflections, and practical guidance."
excerpt: "A collection of video posts by Christopher Sherrod."
preview: "Browse all video posts."
breadcrumbs: true
published: true
toc: false
toc_sticky: false
robots: "index,follow"
---

{% assign video_posts = site.posts | where: "post_type", "video" | sort: "date" | reverse %}
{% include documents-collection.html entries=video_posts type="list" %}
