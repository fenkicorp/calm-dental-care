---
layout: page
title: The Clinic
permalink: /about/clinic/
order: 2
---

  {% for member in site.clinicrooms %}
  <div class="row">

  <div class="col-12 mt-3">
    <div class="card">
      <div class="row justify-content-center">
        <div class="col-6 col-lg-6 mt-3 mt-lg-0">
          <img class="card-img-top animated fadeIn" src="{{ member.image1 }}" >
        </div>
        <div class="col-6 col-lg-6 mt-3 mt-lg-0">
          <img class="card-img-top animated fadeIn" src="{{ member.image2 }}" >
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




  </div>
  {% endfor %}
