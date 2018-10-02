---
layout: default
title: Products
ref: products
lang: en
permalink: /products/

description: An Internet of Things platform and technology company
---

{% include block-0.html %}
{% include block-title.html title=page.title description=page.description %}

<section class="ftco-section ftco-degree-bg" style="padding: 0 0 8em 0;">
    <div class="container">
        <div class="row">
            {% for product in site.products %}
            <div class="col-md-4 ftco-animate">
                <div class="blog-entry">
                    <a href="{{ product.url | prepend: site.baseurl }}" class="block-20" style="background-image: url('{{ product.image | prepend: site.baseurl }}');">
                    </a>
                    <div class="text p-4 d-block">
                        <h3 class="heading"><a href="{{ blog.url | prepend: site.baseurl }}">{{ product.title }}</a></h3>
                        <div class="meta mb-2">
                            <p>{{ product.description | strip_html | strip_newlines }}</p>
                        </div>
                    </div>
                </div>
            </div>
            {% endfor %}
        </div>
    </div>
</section>
