---
layout: page
title: MCQ Bank
permalink: /mcq-bank/
---

Practice daily high-yield Pharmacy MCQs for rapid revision.

<ul>
  {% assign found_posts = false %}
  
  {% for post in site.posts %}
    {% if post.categories contains 'mcqs' or post.category == 'mcqs' %}
      {% assign found_posts = true %}
      <li>
        <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </li>
    {% endif %}
  {% endfor %}

  {% if found_posts == false %}
    <li>No MCQs posted yet. Check back soon!</li>
  {% endif %}
</ul>
