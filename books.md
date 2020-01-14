---
layout: page
title: books
permalink: /books/
---

I'm trying to read 52 books this year (2020) and will keep track of my progress here.
<div class="note__hr"></div>

{% for book in site.books %}
  <div class="note__date">{{ book.title }} ({{ book.number }})</div>
  <p>{{ book.content | markdownify }}</p>
  <span>[goodreads link]({{ book.link }})</span>
  <div class="note__hr"></div>
{% endfor %}