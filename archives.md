---
layout: default
title:  "Archives"
permalink: /archives/
date:   2016-10-03 14:26:40 +02:00
categories: archives
image: "/assets/deploy-engine.jpg"
---
<div id="top">
<div id="entry">
						<div class="Motor">
							<h2 class="title"><a href="//localhost:4000/archives">Archives</a></h2>
						</div>
							
							
{% for post in site.posts  %}
  {% capture this_year %}{{ post.date | date: "%Y" }}{% endcapture %}

  {% if forloop.first %}
  <h2 id="{{ this_year }}-ref">{{this_year}}</h2>
  <ul class="posts">
  {% else %}
      {% if this_year != last_year %}
      </ul>
      <h2 id="{{ this_year }}-ref">{{this_year}}</h2>
      <ul class="posts">
      {% endif %}
  {% endif %}

    <li>
      <span class="post-date">{{ post.date | date_to_string }} &raquo;</span>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>

  {% if forloop.last %}
    </ul>
  {% endif %}

  {% capture last_year %}{{ this_year }}{% endcapture %}
{% endfor %}
</div></div>



		
							

