---
layout: default
title: global.events
icon: fas fas-user
link_key: global.events
namespace: events
permalink: /events/
permalink_de: /Veranstaltungen/
---


<table class="table">
  <thead>
    <tr>
      <th>Sport</th>
      <th>Time</th>
      <th>Location</th>
    </tr>
  </thead>
  <tbody>
     {% for v in site.data.fixtures %}
    <tr>
      <td>
      {% assign sport = site.data.sportTypes[v.sportId] %}
      {% capture sportTranslated %}{% translate sport.key %}{% endcapture %}
              {{ sportTranslated}}
      </td>
      <td>
          {{v.datetime | time_to_long_string }}
      </td>
      <td>
      {% assign venue = site.data.venues[v.venueId] %}
      {{venue.name}}
      </td>
    </tr>
     {% endfor %}
     </tbody>
</table>
