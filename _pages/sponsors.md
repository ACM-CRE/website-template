---
title: Sponsors
lang: en
alternate:
  hi: /hi/sponsors/
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.sponsors.heading }}</h1>

<p class="lead mb-5">We thank our sponsors for making this event possible.</p>

{% include components/sponsor-grid.html %}

<div class="text-center mt-5">
  <h2 class="h4">Become a Sponsor</h2>
  <p>Interested in sponsoring {{ site.data.site.event_name }}?</p>
  <a href="mailto:{{ site.data.site.social.email }}" class="btn btn-primary">Contact Us</a>
</div>

</div>
