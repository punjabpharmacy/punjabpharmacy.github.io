
---
layout: page
title: Pharmacognosy
permalink: /pharmacognosy/
---

Access all high-yield notes, MCQs, and detailed notes pdf below .

<ul>
  {% for post in site.categories.pharmacognosy %}
    <li>
      <strong>{{ post.date | date: "%b %d, %Y" }}</strong> &raquo; 
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% else %}
    <li>No notes in this section yet. Check back soon!</li>
  {% endfor %}
</ul>
