---
layout: default
title: Hello, I'm Chris - Christopher Sherrod
permalink: /new-index
---
<div class="home">
  <!-- Latest Post in Essays -->
  <section id="latest-essay">
    <h2>Latest Essay</h2>
    {% assign latest_essay = site.categories.Essays | first %}
    {% if latest_essay %}
      <article>
        <h3><a href="{{ latest_essay.url }}">{{ latest_essay.title }}</a></h3>
        <p>{{ latest_essay.excerpt }}</p>
        <p><small>{{ latest_essay.date | date: "%B %d, %Y" }}</small></p>
        <p><a href="{{ latest_essay.url }}">Read more</a></p>
      </article>
    {% else %}
      <p>No essays available.</p>
    {% endif %}
  </section>

  <!-- Top 10 Tags -->
  <section id="top-tags">
    <h2>Topics</h2>
    {% assign tags = site.tags | sort: 'size' | reverse %}
    <ul>
      {% for tag in tags limit:10 %}
        <li><a href="{{ site.baseurl }}/tag/{{ tag[0] }}">{{ tag[0] }}</a> ({{ tag[1] | size }})</li>
      {% endfor %}
    </ul>
  </section>

  <!-- Latest Post in Poems -->
  <section id="latest-poem">
    <h2>Latest Poem</h2>
    {% assign latest_poem = site.categories.Poems | first %}
    {% if latest_poem %}
      <article>
        <h3><a href="{{ latest_poem.url }}">{{ latest_poem.title }}</a></h3>
        <p>{{ latest_poem.excerpt }}</p>
        <p><small>{{ latest_poem.date | date: "%B %d, %Y" }}</small></p>
        <p><a href="{{ latest_poem.url }}">Read more</a></p>
      </article>
    {% else %}
      <p>No poems available.</p>
    {% endif %}
  </section>
</div>

  <!-- Last 50 Essays -->
  <section id="last-50-essays">
    <h2>Last 50 Essays</h2>
    <ul>
      {% assign essays = site.categories.Essays | slice: 0, 50 %}
      {% for essay in essays %}
        <li>
          <span>{{ essay.date | date: "%B %d, %Y" }}</span> - 
          <a href="{{ essay.url }}">{{ essay.title }}</a>
        </li>
      {% endfor %}
    </ul>
  </section>

## Receive Updates
Follow me via [email](/newsletter/), [RSS](/feed.xml), [Mastodon](https://pkmsocial/@chris).