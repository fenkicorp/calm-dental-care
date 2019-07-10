---
layout: page
title: Dental Team
permalink: /dental/team/
---

<div class="row mt-5">

  {% for member in site.team %}
  <div class="col-4">
    <div class="card">
      <img class="card-img-top" src="{{ member.image }}" alt="Card image">
      <div class="card-body">
        <h4 class="card-title">{{ member.name }}</h4>
        <p class="card-text">
{{ member.description }}</p>
        </div>
    </div>
  </div>


  {% endfor %}


</div>
