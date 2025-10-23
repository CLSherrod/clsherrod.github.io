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
---
<style>
  /* Give the whole form full-bleed width */
  section#newsletter {
    width: 100vw;
    margin-left: calc(50% - 50vw);
    background-color: #40E0D0;
    padding: 3rem 0;
  }

  #newsletterForm {
    max-width: 900px;
    margin: 0 auto;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
  }

  #newsletterForm input[type="text"],
  #newsletterForm input[type="email"] {
    flex: 1 1 280px;
    min-width: 220px;
    padding: 0.8rem;
    border-radius: 6px;
    border: 2px solid #30c5b6;
    font-size: 1rem;
  }

  #newsletterForm input[type="submit"] {
    background-color: #b94b4b;
    color: white;
    font-size: 1.2rem;
    font-weight: 600;
    border: none;
    border-radius: 100px;
    padding: 0.8rem 1.6rem;
    cursor: pointer;
    transition: background-color .3s ease, transform .2s ease;
  }

  #newsletterForm input[type="submit"]:hover {
    background-color: #30c5b6;
    transform: scale(1.05);
  }
</style>

<!-- ===============================
     NEWSLETTER SECTION
     =============================== -->
<section id="newsletter" style="
  width: 100vw;
  margin-left: calc(50% - 50vw);
  background: #40E0D0;
  padding: 3rem 0;
  text-align: center;
">
 <h2 class="hero-title animate-slide-up">Get my daily letter — one grounded idea for living well.</h2>
  <form id="newsletterForm"
        action="https://mail.nanakasha.com/subscribe"
        method="POST"
        accept-charset="utf-8"
        style="
          display: flex;
          flex-wrap: wrap;
          justify-content: center;
          gap: 1rem;
          max-width: 900px;
          margin: 0 auto;
          background: #40E0D0;
        ">
    <input type="text" name="name" placeholder="Your name" required
           style="flex:1 1 280px; min-width:220px; padding:0.8rem;
                  border:2px solid #30c5b6; border-radius:6px;" />
    <input type="email" name="email" placeholder="Your email" required
           style="flex:1 1 280px; min-width:220px; padding:0.8rem;
                  border:2px solid #30c5b6; border-radius:6px;" />
    <input type="hidden" name="list" value="J1vJg86fQyfkjB72mTmpfA" />
    <input type="hidden" name="subform" value="yes" />
    <button type="submit"
            style="background:#b94b4b; color:#fff; font-weight:600;
                   border:none; border-radius:100px;
                   padding:0.8rem 1.6rem; cursor:pointer;
                   transition:background-color .3s ease, transform .2s ease;">
      Subscribe
    </button>
  </form>
  <p style="margin-top:1rem;">No spam. Unsubscribe anytime.</p>
</section>
