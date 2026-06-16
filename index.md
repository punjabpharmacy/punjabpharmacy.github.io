---
layout: default
title: Home
---

<h2>Latest Exam Updates & Study Material</h2>

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% empty %}
    <li>No posts found. Please check your _posts folder!</li>
  {% endfor %}
</ul>
