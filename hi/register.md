---
title: पंजीकरण
lang: hi
permalink: /hi/register/
alternate:
  en: /register/
---

<div class="container py-5">

{% assign strings = site.data.strings.hi %}

<h1>{{ strings.register.heading }}</h1>

<p class="lead mb-4">{{ site.data.site.event_name }} में अपना स्थान सुरक्षित करें।</p>

{% include components/embed-form.html url=site.data.site.registration_form_url %}

<div class="alert alert-info mt-4">
  <h2 class="h5">किसी अन्य पंजीकरण प्रणाली का उपयोग कर रहे हैं?</h2>
  <p class="mb-0">यह टेम्पलेट Tally.so, Google Forms, या किसी भी सेवा से फॉर्म एम्बेड करने का समर्थन करता है। <code>_data/site.yml</code> में <code>registration_form_url</code> अपडेट करें।</p>
</div>

</div>
