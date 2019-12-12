---
layout: page
title: People
permalink: /people/
---

{% for group in site.data.people %}
  <section>
    <h3><u>{{group.name}}</u></h3>
    {% for person in group.people %}
    <div class="profile">
      <img src="{{ site.baseurl }}/img/{{person.image}}" />
      <h4>{{person.name}}</h4>
      <p class="position">{{person.position}}</p>
      <p class="bio">{{person.bio}}</p>
    </div>
    {% endfor %}
  </section>
{% endfor %}
