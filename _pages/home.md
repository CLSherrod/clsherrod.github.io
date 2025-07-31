---
layout: single
classes: wide
title: "Christopher Sherrod"
permalink: /home/
author_profile: false
breadcrumbs: false
toc: false
teaser: /assets/images/home-header2.webp
header:
  overlay_image: /assets/images/home-header2.webp
  overlay_filter: 0.1
  image_description: "Art by Chr1stopher"
  caption: "Art by [**Chr1stopher**](https://chr1stopher.com)"

# SEO overrides
og_image: /assets/images/home-header2.webp
---

## Hi, I'm Christopher

I'm the author of two books: [**How To Create New Business Ideas Based On What You Love**](/business-ideas/) and [**Hiring Virtual Workers For Small Business**](/hiring/). I'm currently editing my next book, [**Unplug: The 3-Step Plan to Protect Your Body from Hidden EMF Radiation and Reclaim Your Health**](/unplug/). I also write [essays](/categories/#essays), [reviews](/categories/#reviews/), and [poems](/categories/#poems). I'm a visual artist known as [Chr♪stopher](https://chr1stopher.com), and I’ve launched several helpful [projects](/projects/). You can learn [more about me here](/about/).

## The Art of Living a Fulfilling Life  
### Join my newsletter for essays, poems, and slow living insights

<form
  action="https://mail.nanakasha.com/subscribe"
  method="POST"
  accept-charset="utf-8"
  class="newsletter-form"
>
  <div class="newsletter-field">
    <label for="name">Name</label>
    <input type="text" name="name" id="name" />
  </div>
&nbsp;
  <div class="newsletter-field">
    <label for="email">Email</label>
    <input type="email" name="email" id="email" />
  </div>

  <div style="display: none">
    <label for="hp">HP</label>
    <input type="text" name="hp" id="hp" />
  </div>

  <input type="hidden" name="list" value="J1vJg86fQyfkjB72mTmpfA" />
  <input type="hidden" name="subform" value="yes" />
&nbsp;
  <input
    type="submit"
    name="submit"
    id="submit"
    value="Subscribe"
    class="newsletter-submit"
  />
</form>

---

## Latest Writings

<article>
  <ul>
    {% assign sorted_posts = site.posts | sort: 'date' | reverse %}
    {% for post in sorted_posts limit: 10 %}
      <li>
        <strong>{{ post.categories[0] | capitalize }}</strong> – 
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        – <em>{{ post.date | date: "%B %-d, %Y" }}</em>
      </li>
    {% endfor %}
  </ul>
</article>
