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

<div class="row mb-5">
  <div class="col-lg-6 mb-4 mb-lg-0">
    <h2 class="h4">{{ site.data.site.location.name }}</h2>
    <p>{{ site.data.site.location.address }}</p>
    <p>
      <a href="{{ site.data.site.location.url }}" target="_blank" rel="noopener" class="btn btn-outline-primary btn-sm me-2">
        विश्वविद्यालय वेबसाइट पर जाएं
      </a>
      <a href="{{ site.data.site.location.map_url }}" target="_blank" rel="noopener" class="btn btn-outline-secondary btn-sm">
        Google Maps में खोलें
      </a>
    </p>
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

<div class="row mb-5">
  <div class="col-lg-10">
    <h2 class="h4">{{ strings.venue.directions }}</h2>

    <div class="card border-0 bg-light mb-4">
      <div class="card-body">
        <h3 class="h5">विकल्प 1: कार या कैब से</h3>
        <p class="mb-0">अशोका विश्वविद्यालय राजीव गांधी एजुकेशन सिटी में स्थित है, दिल्ली से लगभग 60 किमी दूर। कैंपस NH-44 (पूर्व में NH-1) के माध्यम से पहुंचा जा सकता है। ट्रैफ़िक के आधार पर केंद्रीय दिल्ली या IGI हवाई अड्डे से 1.5-2 घंटे का समय लगता है।</p>
      </div>
    </div>

    <div class="card border-0 bg-light mb-4">
      <div class="card-body">
        <h3 class="h5">विकल्प 2: आज़ादपुर मेट्रो से विश्वविद्यालय शटल</h3>
        <p>अशोका कैंपस के लिए प्रति घंटे शटल <strong>आज़ादपुर मेट्रो स्टेशन गेट 1</strong> से <strong>सुबह 7:30 बजे</strong> से चलती हैं। यात्रा का समय 40 मिनट से 1 घंटे तक है।</p>

        <h4 class="h6 mt-3">इंदिरा गांधी अंतर्राष्ट्रीय हवाई अड्डे से</h4>
        <ul>
          <li><strong>टर्मिनल 1:</strong> T1 मेट्रो स्टेशन से मैजेंटा लाइन लेकर हौज़ खास जाएं। येलो लाइन (समयपुर बादली की ओर) में बदलें और आज़ादपुर पर उतरें।</li>
          <li><strong>टर्मिनल 2 और 3:</strong> T3 से एयरपोर्ट एक्सप्रेस (ऑरेंज लाइन) लेकर नई दिल्ली स्टेशन जाएं। येलो लाइन (समयपुर बादली की ओर) में बदलें और आज़ादपुर पर उतरें।</li>
        </ul>

        <h4 class="h6 mt-3">नई दिल्ली रेलवे स्टेशन से</h4>
        <ul class="mb-0">
          <li>स्टेशन से बाहर निकलें और नई दिल्ली मेट्रो स्टेशन जाएं। येलो लाइन (समयपुर बादली की ओर) सीधे आज़ादपुर तक ले जाएं।</li>
        </ul>

        <p class="small text-muted mt-3 mb-0">मेट्रो प्रवेश द्वार और शटल बोर्डिंग पॉइंट के पास नेवी ब्लू यूनिफॉर्म में विश्वविद्यालय सुरक्षा कर्मचारी सहायता के लिए उपलब्ध हैं।</p>
      </div>
    </div>
  </div>
</div>

{% if site.data.site.accommodation.available %}
<div class="row mb-5">
  <div class="col-lg-8">
    <div class="card border-0 bg-light">
      <div class="card-body">
        <h2 class="h5 mb-3">आवास</h2>
        <p>यदि आपको आवास की आवश्यकता है, तो {{ site.data.site.accommodation.location }} में <strong>{{ site.data.site.accommodation.name }}</strong> उपलब्ध है।</p>
        <p class="mb-0"><strong>दर:</strong> {{ site.data.site.accommodation.price }}</p>
        <p class="small text-muted mt-3 mb-0">बुकिंग सहायता के लिए आयोजकों से संपर्क करें।</p>
      </div>
    </div>
  </div>
</div>
{% endif %}

<div class="row">
  <div class="col-lg-8">
    <div class="card border-primary">
      <div class="card-body">
        <h2 class="h5 mb-3">भागीदारी प्रमाणपत्र</h2>
        <p class="mb-0">सभी प्रतिभागियों को इस कार्यक्रम के हिस्से के रूप में कार्यशाला में भाग लेने का प्रमाणपत्र मिलेगा।</p>
      </div>
    </div>
  </div>
</div>

</div>
