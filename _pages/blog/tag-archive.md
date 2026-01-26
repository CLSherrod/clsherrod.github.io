---
title: "Posts by Tag"
permalink: /tags/
layout: single
author_profile: true
published: false
breadcrumb_parent_title: Blog
breadcrumb_parent_url: /blog/
teaser: /assets/images/teasers/christopher-sherrod-essays-fulfilling-life-square.webp
header:
  overlay_image: /assets/images/headers/tags-header.webp
  overlay_filter: 0.1
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"
---

[Categories](/blog/) · [Years](/years/) · Tags

<div class="taxonomy__index">

{% assign tags = site.tags | sort %}

  <ul class="taxonomy__list">
    {% for tag in tags %}
      <li>
        <a href="{{ site.baseurl }}/tags/#{{ tag[0] | slugify }}">
          <strong>{{ tag[0] }}</strong>
          <span class="taxonomy__count">{{ tag[1].size }}</span>
        </a>
      </li>
    {% endfor %}
  </ul>

</div>
