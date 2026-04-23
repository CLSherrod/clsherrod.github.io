---
title: "Essays by Year"
permalink: /essays/

layout: posts
author_profile: true
breadcrumbs: true

published: true

teaser: /assets/images/teasers/christopher-sherrod-essays-fulfilling-life-square.webp
header:
  overlay_image: /assets/images/headers/blog-header.webp
  overlay_filter: 0.1
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"
---

{%- comment -%}
Optional: if you ALSO want the page to include the year headings (still Liquid-only),
uncomment the block below. If you truly want "just the years", delete everything below.
{%- endcomment -%}

{%- comment -%}
{% for y in years %}

  <h2 id="{{ y.name }}">{{ y.name }}</h2>
{% endfor %}
{%- endcomment -%}
