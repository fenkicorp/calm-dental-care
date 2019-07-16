---
layout: page
title: Treatments
permalink: /treatments/
---
## Treatments


<table class="table table-striped">
<tbody>
{% assign orderedTreatments = site.treatments | sort:"order"%}
{% for t in orderedTreatments %}
  <tr>
    <td><a href="{{t.url}}">{{t.title}}</a></td>
    <td>{{t.description}}</td>
  </tr>
{% endfor %}
</tbody>
</table>
