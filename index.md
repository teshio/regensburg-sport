---
layout: default
namespace: home
permalink: /
permalink_de: /
title: global.home
---

<div class="row justify-content-center mb-3">
  <div class="col-2 text-center">
    <img src="/assets/images/logo.jpg" class="img-thumbnail" />
  </div>
</div>
<div class="row mb-5">
  <div class="col-12 text-center">
    <h3>sdWM 2019</h3>
    {% t 'pages.home' %}
  </div>
</div>

<div class="jumbotron bg-dark text-white">
  <div class="col-12">
        {% tf home/whenandwhere.md %}
  </div>
</div>


<div class="row mb-3">
  <div class="col-md-4">
    <div class="card" >
      <img src="/assets/images/register.jpg" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">Registration</h5>
          <ul>
            <li>70€ für Stips</li>
            <li>80€ Alumni / Geschäftsstelle</li>
            <li>90€ Externe</li>
            <li>30€ ohne Übernachtung</li>
          </ul>

        <p class="card-text">
          Single registrations are welcome too.
        </p>
        <a target="_register" href="https://docs.google.com/forms/d/e/1FAIpQLSfZye6qEJ3gmfbC0zrlO83qT5J5U72q9El2a7wpoJ77s6GLZg/viewform?fbclid=IwAR26JC8S-Mh14wkxaJFj5T3VTx6YYotE0sKY5BxSrSkkVYNDjBQX1E4sem0" class="btn btn-primary">Register now!</a>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card" >
      <img src="/assets/images/accomodation.jpg" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">{% t 'global.accomodation' %}</h5>

        <p class="card-text">
          {% t pages.accomodation %}
        </p>
        <a href="{% tl accomodation %}" class="btn btn-primary">{% t 'global.moreinfo' %}</a>
      </div>
    </div>
  </div>
  <div class="col-md-4">
    <div class="card" >
      <img src="/assets/images/map.png" class="card-img-top" alt="...">
      <div class="card-body">
        <h5 class="card-title">{% t 'global.gettingthere' %}</h5>

        <p class="card-text">
          {% t pages.gettingthere %}
        </p>
        <a href="{% tl accomodation %}" class="btn btn-primary">{% t 'global.moreinfo' %}</a>
      </div>
    </div>
  </div>
</div>


<div class="card">
  <div class="card-body">

    <div class="row">
      <div class="col-6">
        <img src="/assets/images/sports-main.jpg" class="img-thumbnail" />
      </div>
      <div class="col-6">
          {% tf home/programme.md %}
        <a href="{% tl events %}" class="btn btn-primary">{% t 'global.moreinfo' %} </a>
      </div>
    </div>
  </div>

</div>
