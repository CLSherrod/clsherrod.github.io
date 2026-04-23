---
title: "News"
tagline: "Read updates and announcements from Christopher Sherrod."
layout: archive
permalink: /news/
description: "Browse news, updates, and announcements from Christopher Sherrod."
excerpt: "A collection of news and updates from Christopher Sherrod."
preview: "Browse all news posts."
breadcrumbs: true
published: true
toc: false
toc_sticky: false
robots: "index,follow"
---

{% assign news_posts = site.posts | where: "post_type", "news" | sort: "date" | reverse %}
{% include documents-collection.html entries=news_posts type="list" %}
