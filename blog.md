---
layout: default
title: Blog
permalink: /blog/
---

<div class="home">

  <h1 class="page-heading" style="color: #F91414">Posts</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
      <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ excerpt }}{{ post.title | escape }}</a>
        </h2>
	
      </li><br>
    {% endfor %}
  </ul>
  

  <p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

</div>
