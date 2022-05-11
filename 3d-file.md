---
layout: page
title: 3D printable files
---

## Available 3D-printable files



<div>
{% for resource in site.resources %}
{% if resource.type == "3d-file" %}
    <div class="col-md col-sm-11 portfolio-item effect1">
        <a href="#r{{ forloop.index }}" class="portfolio-link" data-toggle="modal">
            <img src="{{ resource.image }}" class="img-fluid grid-img" alt="">
            <div class="portfolio-caption">
                <h4>{{ resource.title }}</h4>
                <p class="text-muted">{{ resource.description }}</p>
           </div>
        </a>                  
    </div>
{% endif %}
{% endfor %}
</div>

{% include resourcemodals.html %}