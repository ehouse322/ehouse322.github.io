---
layout: page
title: thoughts
permalink: /thoughts/
---

For quickly jotting down thoughts or short notes I want to remember
<div class="thought__hr"></div>


{% for thought in site.thoughts %}
  <div class="thought__date">{{ thought.date | date: "%-d %b %Y -- %H:%M" }}</div>
  <p>{{ thought.content | markdownify }}</p>
  <div class="thought__hr"></div>
{% endfor %}