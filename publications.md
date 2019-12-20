---
layout: page
title: Publications
permalink: /publications/
---
<section class="collection">
  <h2 class="underline">Selected Publications</h2>
  {% for pub in site.data.pub_peer_reviewed %}
    <div class="publication">
      <h4>{{pub.title}}</h4>
      <p>
        <label>Published in: </label><span>{{pub.publication}}</span><br/>
        <label>Authors: </label><span>{{pub.authors}}</span><br/>
      </p>
      {% if pub.doi %}
        <a href="https://doi.org/{{pub.doi}}">{{pub.doi}}</a> | 
      {% endif %}
      <a href="{{pub.url}}">{{pub.url}}</a>
    </div>
  {% endfor %}
</section>
<hr>
<section class="collection">
  <h2 class="underline">Formal Expert Group / Policy Evidence</h2>
  {% for pub in site.data.pub_fegpe %}
    <div class="publication">
      <h4>{{pub.event}}</h4>
      <p><label>Speaker:</label><span>{{pub.speaker}}</span></p>
      {% if pub.url %}
        <a href="{{pub.url}}">{{pub.url}}</a>
      {% endif %}
    </div>
  {% endfor %}
</section>
<hr>
<section class="collection">
  <h2 class="underline">Keynotes and Invited Talks</h2>
  {% for pub in site.data.pub_keynotes %}
    <div class="publication">
      <h4>{{pub.title}}</h4>
      <p>
        <label>Event:</label><span>{{pub.event}}</span><br/>
        <label>Speaker:</label><span>{{pub.speaker}}</span>
      </p>
      {% if pub.url %}
        <a href="{{pub.url}}">{{pub.url}}</a>
      {% endif %}
    </div>
  {% endfor %}
</section>
<hr>
<section class="collection">
  <h2 class="underline">Blog Posts</h2>
  {% for pub in site.data.pub_blog %}
    <div class="publication">
      <h4>{{pub.title}}</h4>
      {% if pub.url %}
        <a href="{{pub.url}}">{{pub.url}}</a>
      {% endif %}
    </div>
  {% endfor %}
</section>
