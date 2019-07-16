---
layout: page
title: Dental Team
permalink: /about/team/
order: 3
---

<div class="row mt-5">

  {% for member in site.team %}
  <div class="col-4">
    <div class="card">
      <img class="card-img-top animated fadeIn" src="{{ member.image }}" alt="Card image">
      <div class="card-body">
        <h4 class="card-title">{{ member.name }}</h4>
                <h5 class="card-title">{{ member.title }}</h5>
                <h6 class="card-title">{{ member.qualifications }}</h6>
        <p class="card-text">
{{ member.description }}</p>
        </div>
    </div>
  </div>


  {% endfor %}


</div>
