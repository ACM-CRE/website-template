---
title: Venue
lang: en
alternate:
  hi: /hi/venue/
---

<div class="container py-5">

{% assign lang = page.lang | default: site.lang | default: "en" %}
{% assign strings = site.data.strings[lang] %}

<h1>{{ strings.venue.heading }}</h1>

<div class="row mb-5">
  <div class="col-lg-6 mb-4 mb-lg-0">
    <h2 class="h4">{{ site.data.site.location.name }}</h2>
    <p>{{ site.data.site.location.address }}</p>
    <p>
      <a href="{{ site.data.site.location.url }}" target="_blank" rel="noopener" class="btn btn-outline-primary btn-sm me-2">
        Visit University Website
      </a>
      <a href="{{ site.data.site.location.map_url }}" target="_blank" rel="noopener" class="btn btn-outline-secondary btn-sm">
        Open in Google Maps
      </a>
    </p>
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

<div class="row mb-5">
  <div class="col-lg-10">
    <h2 class="h4">{{ strings.venue.directions }}</h2>

    <div class="card border-0 bg-light mb-4">
      <div class="card-body">
        <h3 class="h5">Option 1: By Car or Cab</h3>
        <p class="mb-0">Ashoka University is located in Rajiv Gandhi Education City, approximately 60 km from Delhi. The campus is accessible via NH-44 (formerly NH-1). Expect 1.5–2 hours from central Delhi or IGI Airport depending on traffic.</p>
      </div>
    </div>

    <div class="card border-0 bg-light mb-4">
      <div class="card-body">
        <h3 class="h5">Option 2: University Shuttle from Azadpur Metro</h3>
        <p>Hourly shuttles to the Ashoka campus run from <strong>Azadpur Metro Station Gate 1</strong> starting at <strong>7:30 AM</strong>. Travel time is 40 minutes to 1 hour.</p>

        <h4 class="h6 mt-3">From Indira Gandhi International Airport</h4>
        <ul>
          <li><strong>Terminal 1:</strong> Take the Magenta Line from T1 Metro Station to Hauz Khas. Switch to the Yellow Line (towards Samaypur Badli) and get off at Azadpur.</li>
          <li><strong>Terminals 2 & 3:</strong> Take the Airport Express (Orange Line) from T3 to New Delhi Station. Switch to the Yellow Line (towards Samaypur Badli) and get off at Azadpur.</li>
        </ul>

        <h4 class="h6 mt-3">From New Delhi Railway Station</h4>
        <ul class="mb-0">
          <li>Exit the station and head to New Delhi Metro Station. Take the Yellow Line (towards Samaypur Badli) directly to Azadpur.</li>
        </ul>

        <p class="small text-muted mt-3 mb-0">University security staff in navy blue uniforms are available near the metro entrance and shuttle boarding point for assistance.</p>
      </div>
    </div>
  </div>
</div>

{% if site.data.site.accommodation.available %}
<div class="row mb-5">
  <div class="col-lg-8">
    <div class="card border-0 bg-light">
      <div class="card-body">
        <h2 class="h5 mb-3">Accommodation</h2>
        <p>If you need accommodation, the <strong>{{ site.data.site.accommodation.name }}</strong> at {{ site.data.site.accommodation.location }} is available.</p>
        <p class="mb-0"><strong>Rate:</strong> {{ site.data.site.accommodation.price }}</p>
        <p class="small text-muted mt-3 mb-0">Contact the organizers for booking assistance.</p>
      </div>
    </div>
  </div>
</div>
{% endif %}

<div class="row">
  <div class="col-lg-8">
    <div class="card border-primary">
      <div class="card-body">
        <h2 class="h5 mb-3">Certificate of Participation</h2>
        <p class="mb-0">All participants will receive a certificate for attending the workshop as part of this event.</p>
      </div>
    </div>
  </div>
</div>

</div>
