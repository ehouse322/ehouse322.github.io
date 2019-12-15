---
layout: page
title: notes
permalink: /notes/
---

For quickly jotting down thoughts or short notes I want to remember
<div class="note__hr"></div>


{% for note in site.notes reversed %}
  <div class="note__date">{{ note.date | date: "%-d %b %Y -- %H:%M" }}</div>
  <p>{{ note.content | markdownify }}</p>
  <div class="note__hr"></div>
{% endfor %}