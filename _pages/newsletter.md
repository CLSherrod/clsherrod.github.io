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

  <!-- Newsletter -->
<section
  id="newsletter"
  style="background-color: turquoise; padding: 20px; border-radius: 8px"
>
  <br />
  <p
    style="
      text-align: center;
      font-size: 1.5rem;
      margin-bottom: 10px;
      font-weight: bold;
    "
  >
    We're here to talk about living a fulfilling life.
  </p>

      <form
        id="newsletterForm"
        action="https://mail.nanakasha.com/subscribe"
        method="POST"
        accept-charset="utf-8"
        style="
          display: flex;
          flex-wrap: wrap;
          justify-content: center;
          gap: 15px;
          background-color: turquoise;
          padding: 20px;
          border-radius: 8px;
          max-width: 600px;
          margin: 0 auto;
        "
      >
        <div
          style="
            display: flex;
            flex-direction: column;
            flex: 1 1 250px;
            min-width: 220px;
          "
        >
          <label for="name" style="margin-bottom: 5px; font-weight: bold">Name</label>
          <input
            type="text"
            name="name"
            id="name"
            required
            autocomplete="name"
            style="
              border: 2px solid blue;
              padding: 10px;
              border-radius: 5px;
              font-size: 1rem;
              width: 100%;
              box-sizing: border-box;
            "
          />
        </div>

        <div
          style="
            display: flex;
            flex-direction: column;
            flex: 1 1 250px;
            min-width: 220px;
          "
        >
          <label for="email" style="margin-bottom: 5px; font-weight: bold">Email</label>
          <input
            type="email"
            name="email"
            id="email"
            required
            autocomplete="email"
            inputmode="email"
            style="
              border: 2px solid blue;
              padding: 10px;
              border-radius: 5px;
              font-size: 1rem;
              width: 100%;
              box-sizing: border-box;
            "
          />
        </div>

        <!-- Honeypot field (hidden from users & assistive tech) -->
        <div style="position: absolute; left: -9999px;" aria-hidden="true">
          <label for="website" title="Leave this field blank">Website</label>
          <input
            type="text"
            name="website"
            id="website"
            tabindex="-1"
            autocomplete="off"
          />
        </div>

        <!-- Timestamp field (hidden) -->
        <input type="hidden" name="timestamp" id="timestamp" />

        <input type="hidden" name="list" value="J1vJg86fQyfkjB72mTmpfA" />
        <input type="hidden" name="subform" value="yes" />

        <!-- Centered responsive submit button -->
        <div
          style="
            display: flex;
            justify-content: center;
            margin-top: 10px;
            width: 100%;
          "
        >
          <input
            type="submit"
            name="submit"
            id="submit"
            value="Subscribe"
            style="
              border: 0;
              padding: 0.8em 1.4em;
              background-color: rgb(185, 75, 75);
              color: white;
              cursor: pointer;
              border-radius: 100px;
              width: 100%;
              max-width: 220px;
              font-size: 1.5rem;
              font-weight: 600;
              letter-spacing: -0.004em;
              line-height: 1;
              display: inline-flex;
              align-items: center;
              justify-content: center;
              gap: 0.4em;
              margin: 0 auto;
            "
          />
        </div>
      </form>

      <script>
        (function () {
          function init() {
            var ts = document.getElementById("timestamp");
            if (ts) ts.value = Date.now();

            var form = document.getElementById("newsletterForm");
            if (!form) return;

            form.addEventListener("submit", function (e) {
              var tsEl = document.getElementById("timestamp");
              var start = parseInt(tsEl && tsEl.value ? tsEl.value : "0", 10);
              var elapsed = start ? (Date.now() - start) / 1000 : 999; // allow submission if JS failed
              var honeypotEl = document.getElementById("website");
              var honey = honeypotEl && honeypotEl.value ? honeypotEl.value : "";

              if (honey !== "" || elapsed < 5) {
                e.preventDefault();
                console.warn("Spam submission blocked.");
                return false;
              }
            });
          }

          if (document.readyState === "loading") {
            document.addEventListener("DOMContentLoaded", init);
          } else {
            init();
          }
        })();
      </script>
</section>

  <hr>
  <!-- Intro -->
  <section id="intro">
    I am the author of two books on
    <a href="/business-ideas/"
      >How To Create New Business Ideas Based On What You Love</a
    >, plus numerous <a href="/categories/#essays">essays</a>,
    <a href="/categories/#reviews">reviews</a>, and
    <a href="/categories/#poems">poems</a>. I am also a
    <a href="/whodefinesyou/">web agency</a> owner, artist and musician
    <a href="/chr1stopher/">Chr♪stopher</a> and some helpful
    <a href="/projects/">projects</a>.<br /><br />
  </section>
