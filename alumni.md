---
title: LBR Alumni
layout: page
---

### LBR Alumni

LBR is most grateful for all of the alumni that contributed to making this lab what it is. 

<div class="row">
    {% for person in site.alumni %}
    <div class="col-sm-3">
      <div class="team-member">
      <a class="portfolio-link" data-toggle="modal" href="#p{{ forloop.index }}">
        <img class="mx-auto rounded-circle" src="{{ person.image }}" alt="">
      </a>
      <h4>{{ person.name }}</h4>
      <p class="text-muted">{{ person.role }}</p>
      <ul class="list-inline social-buttons">
      {% for network in person.social %}
      {%- if network.url -%}  
      <li class="list-inline-item">
        <a href="{{ network.url }}">
          <i class="{{ network.icon }}"></i>
        </a>
        </li>
      {%- endif -%}
      {% endfor %}
      </ul>
      </div>
    </div>
    {% endfor %}
</div>