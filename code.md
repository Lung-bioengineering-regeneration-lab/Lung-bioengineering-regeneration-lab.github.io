---
layout: page
title: Bioinformatics Piplines
---

## LBR Bioinformatics piplines

This page contains the most updated LBR bioinformatics pipelines


<div>
{% for resource in site.resources %}
{% if resource.type == "code" %}
    <div class="col-md col-sm-11 portfolio-item effect1">
        <a href="#r{{ forloop.index }}" class="portfolio-link" data-toggle="modal">
            <img src="{{ resource.image }}" class="img-fluid grid-img" alt="">
            <div class="portfolio-caption">
                <h4>{{ resource.title }}</h4>
                <p class="text-muted">{{ resource.subtitle }}</p>
           </div>
        </a>                  
    </div>
{% endif %}
{% endfor %}
</div>

{% include resourcemodals.html %}