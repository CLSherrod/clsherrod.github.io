---
layout: single
title: What I'm Doing Now
permalink: /now/

breadcrumbs: true

toc: true
teaser: /assets/images/teasers/christopher-sherrod-essays-fulfilling-life-square.webp
header:
  overlay_image: /assets/images/headers/now-header.webp
  overlay_filter: 0.1
  image_description: "Art Time by Chr1stopher"
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"
# SEO overrides
og_image: /assets/images/now-header.webp
---

_Updated on {{ site.time | date: "%A, %B %-d, %Y" }}_

Lately I’ve been thinking a lot about how much better life gets when you stop trying to optimize everything and start paying closer attention to what actually nourishes you.

Here’s what I’m focused on lately: what I’m building, what I’m writing, and what has my attention right now.

## What I’m Focused On

I’m finishing [_Unplug: The 4-Step Plan_](/courses/unplug/), my course on reducing EMF exposure and rebuilding daily life around clearer choices and better health.

## What I’m Making

- Writing essays on what has worked for me in life, work, and paying closer attention.
- I'm an artist known as [Chr1stopher](/chr1stopher).

## Start Here

- [The Dented Ping Pong Ball and the Beauty of an Unplanned Life](https://christophersherrod.com/dented-ping-pong-ball-fulfilling-life/)
- [Why I Don’t Care About Slow Living or Fast Living — I Care About Feeling Fulfilled](https://christophersherrod.com/fulfilled-not-fast-or-slow/)
- [Finding Balance: Why Extreme Mindsets Don’t Lead to Success](https://christophersherrod.com/finding-balance/)

## Recent Writing

I’m also writing essays on living a fulfilling life, meaningful work, and the quieter changes that make daily life feel more like your own.

{% assign filtered_posts = site.posts
  | where_exp: "post", "post.post_type != 'poem'"
  | where_exp: "post", "post.post_type != 'review'"
  | where_exp: "post", "post.post_type != 'news'"
  | where_exp: "post", "post.post_type != 'video'"
  | sort: "date"
  | reverse
%}

<ul class="now-posts-list">
  {% for post in filtered_posts limit: 5 %}
    <li class="now-post-item">
      <a class="now-post-title" href="{{ post.url | relative_url }}">
        {{ post.title | escape }}
      </a> -
      <span class="now-post-date">
        {{ post.date | date: "%B %d, %Y" }}
      </span>
    </li>
  {% endfor %}
</ul>

See my [past essays](/essays/)

## What I’ve Been Enjoying

A few things I’ve been enjoying or returning to lately:

- Books I’ve read over the years are listed on [my Goodreads profile](https://www.goodreads.com/christophersherrod).
- I recommend the [1001 Albums You Must Hear Before You Die challenge](https://1001albumsgenerator.com/shares/6093ff2a336e5a7f8b50c476). I enjoyed it so much I wrote an [entire essay about it](/1001-albums/).
- You can also browse [what I’ve been listening to on Apple Music](https://music.apple.com/profile/clsherrod)
- [My past movie ratings on IMDb](https://www.imdb.com/user/ur119282955/ratings).

## Join The Daily Note

If you’d like the quieter, ongoing version of this page, join my [daily note](/newsletter/).
