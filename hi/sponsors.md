---
title: प्रायोजक
lang: hi
permalink: /hi/sponsors/
alternate:
  en: /sponsors/
---

<div class="container py-5">

{% assign strings = site.data.strings.hi %}

<h1>{{ strings.sponsors.heading }}</h1>

<p class="lead mb-5">इस कार्यक्रम को संभव बनाने के लिए हम अपने प्रायोजकों का धन्यवाद करते हैं।</p>

{% include components/sponsor-grid.html %}

<div class="text-center mt-5">
  <h2 class="h4">प्रायोजक बनें</h2>
  <p>{{ site.data.site.event_name }} को प्रायोजित करने में रुचि रखते हैं?</p>
  <a href="mailto:{{ site.data.site.social.email }}" class="btn btn-primary">संपर्क करें</a>
</div>

</div>
