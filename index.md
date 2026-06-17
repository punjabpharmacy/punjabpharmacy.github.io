---
layout: default
title: Home
---

<p>
  <strong>Quick Links:</strong> 
  <a href="{{ '/pharmacology/' | relative_url }}">Pharmacology</a> | 
  <a href="{{ '/jurisprudence/' | relative_url }}">Jurisprudence</a> | 
  <a href="{{ '/mcq-bank/' | relative_url }}">MCQ Bank</a>
</p>
<hr>
<h2>Latest Exam Updates & Study Material</h2>

<ul>
  {% for post in site.posts %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% else %}
    <li>No posts found. Please check your _posts folder!</li>
  {% endfor %}
</ul>
---
---

<p style="text-align: center; font-size: 0.9em;">
  &copy; 2026 Punjab Pharmacy | 
  <a href="{{ '/about/' | relative_url }}">About Us</a> | 
  <a href="{{ '/contact/' | relative_url }}">Contact Us</a> | 
  <a href="{{ '/privacy-policy/' | relative_url }}">Privacy Policy</a> | 
  <a href="{{ '/disclaimer/' | relative_url }}">Disclaimer</a>
</p>
