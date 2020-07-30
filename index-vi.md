---
layout: default
title: Ubisen | Trang chủ
ref: index
lang: vi
permalink: /vi/
image: /images/services/agriculture.jpg
---

{% include block-welcome.html data=site.data.home.welcome-vi %}

<!-- {% include block-slider.html data=site.data.home.slider %} -->

{% include block-4.html data=site.data.home.block-4-vi %}

<!-- {% assign solutions = site.solutions | where_exp:"item", "item.lang == page.lang" %} -->

<!-- {% include block-2.html title="An Internet of Things platform and technology" description="Use cases" contents=solutions %} -->

<!-- {% include block-number.html data=site.data.home.block-number-vi %} -->

<!-- {% include block-3.html title="An Internet of Things platform and technology" description="Use cases" contents=solutions %} -->

{% include block-content-slider.html title="An Internet of Things platform and technology" description="Use cases" contents=solutions %}
