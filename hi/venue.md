---
title: स्थान
lang: hi
permalink: /hi/venue/
alternate:
  en: /venue/
---

<div class="container py-5">

{% assign strings = site.data.strings.hi %}

<h1>{{ strings.venue.heading }}</h1>

<div class="row">
  <div class="col-lg-6 mb-4">
    <h2 class="h4">{{ site.data.site.location.name }}</h2>
    <p>{{ site.data.site.location.address }}</p>

    <h3 class="h5 mt-4">{{ strings.venue.directions }}</h3>
    <p>स्थल तक पहुंचने, पार्किंग, सार्वजनिक परिवहन आदि के बारे में विवरण।</p>
  </div>

  <div class="col-lg-6">
    {% if site.data.site.location.map_embed_url %}
      <div class="venue-map">
        <iframe
          src="{{ site.data.site.location.map_embed_url }}"
          title="स्थान का नक्शा"
          loading="lazy"
          allowfullscreen>
        </iframe>
      </div>
    {% endif %}
  </div>
</div>

</div>
