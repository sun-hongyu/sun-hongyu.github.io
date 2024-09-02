---
title: "CV"
layout: gridlay
sitemap: false
permalink: /CV/
---

<!-- #### Short c.v. -->

{% for member in site.data.pi %}

<div class="jumbotron" style="background-color: transparent; border: none;">
<div class="row">
<div class="col-sm-4">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-8 col-xs-12">
  <h4>{{ member.name }}</h4>
  <!-- <h2><i>{{ member.info }}</i></h4> -->
   {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
   {% if member.orcid %} <a href="{{ member.orcid }}" target="_blank"><i class="ai ai-orcid-square ai-3x"></i></a> {% endif %}
   {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %}
   {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
   {% if member.linkedin %} <a href="{{ member.linkedin }}" target="_blank"><i class="fa fa-linkedin-square ai-3x"></i></a> {% endif %}
  
  <h4>Education</h4>

  <ul style="overflow: hidden">
    {% for education in member.education %}
      <li>{{ education | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

  <h4>Professional Appointments</h4>

  <ul style="overflow: hidden">
    {% for appointment in member.appointment %}
      <li>{{ appointment | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

  <h4>Academic Services</h4>

  <ul style="overflow: hidden">
    {% for service in member.service %}
      <li>{{ service | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

  <h4>Awards</h4>

  <ul style="overflow: hidden">
    {% for award in member.award %}
      <li>{{ award | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

</div>
</div>
</div>
{% endfor %}

<!-- {% if site.data.grants %}

<div class="jumbotron">
  <h3>Academic Services</h3>
  <ul>
    {% for grant in site.data.grants %}
      <li>{{ grant.name }}</li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if site.data.awards %} -->

<!-- <div class="jumbotron">
  <h3>Awards</h3>
  <ul>
    {% for award in site.data.awards %}
      <li>{{ award.name | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>
</div>
{% endif %}

{% if site.data.people %} -->

<!-- <div class="jumbotron">
  <h3>Students and Mentoring</h3>
  <ul>
    {% for student in site.data.people %}
      <li>{{ student.name }}, {{ student.location }} ({{ student.degree }}, {{ student.year }})</li>
    {% endfor %}
  </ul>
</div>
{% endif %} -->

<!-- <div class="jumbotron">
  <h4>Sponsors</h4>
  <div style='display:block; text-align:center; margin-left:auto; margin-right:auto;'>
  {% for funder in site.data.funders %}<a href="{{ funder.url }}" target="_blank"><img src='{{ site.url }}{{ site.baseurl }}/images/{{ funder.image }}' style='max-height: 80px; max-width: 200px; margin: 1%'/></a>{% endfor %}
  </div>
</div> -->
