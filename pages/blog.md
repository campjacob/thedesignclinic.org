---
layout: page
title: The Design Fix
permalink: /blog/
---

<h1>{{ page.title }}</h1>

<ul>
  {% for post in site.posts %}
    <li class="post" style="list-style: none;">
      <h3><a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
    
      {{ post.content }}
    </li>
  {% endfor %}
</ul>


<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>

