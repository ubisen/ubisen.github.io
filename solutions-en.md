---
layout: default
title: Solutions
ref: solutions
lang: en
permalink: /solutions/
description: Ubisen solutions
---

{% include block-0.html %}
{% include block-title.html title=page.title description=page.description %}

{% assign solutions = site.solutions | where_exp:"item", "item.lang == page.lang" %}
<section class="ftco-section ftco-degree-bg" style="padding: 0 0 8em 0;">
    <div class="container">
        <div class="row">
            {% for solution in solutions %}
            <div class="col-md-4 ftco-animate">
                <div class="blog-entry">
                    <a href="{{ solution.url | prepend: site.baseurl }}" class="block-20" style="background-image: url('{{ solution.image | prepend: site.baseurl }}');">
                    </a>
                    <div class="text p-4 d-block">
                        <h3 class="heading"><a href="{{ solution.url | prepend: site.baseurl }}">{{ solution.title }}</a></h3>
                        <div class="meta mb-2">
                            <p>{{ solution.description | strip_html | strip_newlines }}</p>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</section>
