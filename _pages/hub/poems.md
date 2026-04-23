---
title: "Poems"
tagline: "Read poems by Christopher Sherrod."
layout: archive
permalink: /poems/
description: "Browse poems by Christopher Sherrod"
excerpt: "A collection of peoms by Christopher Sherrod."
preview: "Browse all poems."
breadcrumbs: true

header:
  overlay_image: /assets/images/headers/blog-header.webp
  overlay_filter: 0.1
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"

published: true

robots: "index,follow"
---

{% assign poem_posts = site.posts | where: "post_type", "poem" | sort: "date" | reverse %}
{% include documents-collection.html entries=poem_posts type="list" %}
