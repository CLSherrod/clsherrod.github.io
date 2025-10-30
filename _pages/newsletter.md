---
layout: single
classes: wide
title: Newsletter
permalink: /newsletter/
teaser: /assets/images/newsletter-header.webp
header:
  overlay_image: /assets/images/newsletter-header.webp
  overlay_filter: 0.1
  image_description: Art Newsletter by Chr1stopher
  caption: Art by [**Chr1stopher**](https://chr1stopher.com)
author_profile: false
redirect_to: "https://christophersherrod.com/#newsletter"
---

<style>
  #newsletterFormWrapper {
    width: 100vw;
    margin-left: calc(50% - 50vw);
    background-color: #40E0D0;
    padding: 3rem 0;
    text-align: center;
  }

  #newsletterFormWrapper form {
    max-width: 900px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
  }

  #newsletterFormWrapper input[type="text"],
  #newsletterFormWrapper input[type="email"] {
    flex: 1 1 280px;
    min-width: 220px;
    padding: 0.8rem;
    border: 2px solid #30c5b6;
    border-radius: 6px;
    font-size: 1rem;
  }

  #newsletterFormWrapper button {
    background-color: #b94b4b;
    color: white;
    font-weight: 600;
    border: none;
    border-radius: 100px;
    padding: 0.8rem 1.6rem;
    cursor: pointer;
    transition: background-color .3s ease, transform .2s ease;
  }

  #newsletterFormWrapper button:hover {
    background-color: #30c5b6;
    transform: scale(1.05);
  }
</style>
<h2 class="hero-title animate-slide-up">Get my daily letter — one grounded idea for living well.</h2>
<section id="newsletterFormWrapper">
  <form action="https://mail.nanakasha.com/subscribe" method="POST">
    <input type="text" name="name" placeholder="Your name" required>
    <input type="email" name="email" placeholder="Your email" required>
    <input type="hidden" name="list" value="J1vJg86fQyfkjB72mTmpfA">
    <input type="hidden" name="subform" value="yes">
    <button type="submit">Subscribe</button>
  </form>
  <p>No spam. Unsubscribe anytime.</p>
</section>
