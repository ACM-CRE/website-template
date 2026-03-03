---
title: Register
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.register.heading }}</h1>

<p class="lead mb-4">Secure your spot at {{ site.data.site.event_name }}.</p>

{% include components/embed-form.html url=site.data.site.registration_form_url %}

<div class="alert alert-info mt-4">
  <h2 class="h5">Using a different registration system?</h2>
  <p class="mb-0">This template supports embedding forms from Tally.so, Google Forms, or any service that provides an embed URL. Update the <code>registration_form_url</code> in <code>_data/site.yml</code>.</p>
</div>

</div>
