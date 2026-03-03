---
title: Speakers
lang: en
alternate:
  hi: /hi/speakers/
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.speakers.heading }}</h1>

<p class="lead mb-4">Meet our speakers and workshop facilitators.</p>

{% include components/speaker-list.html %}

</div>
