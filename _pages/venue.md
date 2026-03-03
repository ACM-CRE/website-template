---
title: Venue
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.venue.heading }}</h1>

<div class="row">
  <div class="col-lg-6 mb-4">
    <h2 class="h4">{{ site.data.site.location.name }}</h2>
    <p>{{ site.data.site.location.address }}</p>

    <h3 class="h5 mt-4">{{ strings.venue.directions }}</h3>
    <p>Details about getting to the venue, parking, public transit, etc.</p>
  </div>

  <div class="col-lg-6">
    {% if site.data.site.location.map_embed_url %}
      <div class="venue-map">
        <iframe
          src="{{ site.data.site.location.map_embed_url }}"
          title="Venue location map"
          loading="lazy"
          allowfullscreen>
        </iframe>
      </div>
    {% endif %}
  </div>
</div>

</div>
