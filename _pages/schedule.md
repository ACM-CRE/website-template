---
title: Schedule
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.schedule.heading }}</h1>

<p class="lead mb-4">{{ site.data.site.date_display }} &middot; {{ site.data.site.time }}</p>

{% include components/schedule-table.html %}

</div>
