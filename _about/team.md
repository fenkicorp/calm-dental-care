---
layout: page
title: Dental Team
permalink: /about/team/
order: 3
---

<div class="row">

  {% for member in site.team %}
  <div class="col-lg-4 mt-3">
    <div class="card">
      <div class="row justify-content-center">
        <div class="col-7 col-lg-12 mt-3 mt-lg-0">
          <img class="card-img-top animated fadeIn" src="{{ member.image }}" alt="Card image">
        </div>
      </div>
      <div class="card-body">
      {% if member.website %}
      <a target="blank" href="{{ member.website }}" class="btn btn-sm btn-primary float-right animated shake"><i class="fas fa-external-link-square-alt"></i></a>
      {% endif %}
        <h4 class="card-title">{{ member.name }}</h4>
                <h5 class="card-title text-secondary">{{ member.title }}</h5>
                <h6 class="card-title text-secondary">{{ member.qualifications }}</h6>
        <p class="card-text">

{{ member.description }}</p>

        </div>
    </div>
  </div>


  {% endfor %}


</div>
