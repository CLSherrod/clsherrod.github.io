---
title: "Reviews"
tagline: "Read reviews by Christopher Sherrod."
layout: archive
permalink: /reviews/
description: "Browse reviews by Christopher Sherrod, including books, media, and other thoughtful recommendations."
excerpt: "A collection of reviews by Christopher Sherrod."
preview: "Browse all reviews."
breadcrumbs: true
published: true
toc: false
toc_sticky: false
robots: "index,follow"
---

{% assign review_posts = site.posts | where: "post_type", "review" | sort: "date" | reverse %}
{% include documents-collection.html entries=review_posts type="list" %}
