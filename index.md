---
layout: default
title: Home
---

<p>
  <strong>Quick Links:</strong> 
  <a href="{{ '/pharmacology/' | relative_url }}">Pharmacology</a> | 
  <a href="#">Pharmaceutics</a> | 
  <a href="#">Job Updates</a>
</p>
<hr>
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
