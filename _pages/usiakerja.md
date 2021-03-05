---
layout: default
title: "Usia Kerja"
permalink: /usiakerja
---
{% assign sorted = site.categories.UsiaKerja | reverse %}

<h4 class="mt-5 mb-neg-30" id="{{ category[0] | replace: " ","-" }}"><span class="text-capitalize badge badge-primary text-small">{{ page.title }}</span></h4>
<div class="blog-grid-container">
    {% for post in sorted %}
    {% if post.title != null %}
    {% include postbox.html %}
    {% endif %}
    {% endfor %}
</div>