---
layout: page
title: books
permalink: /books/
---

Books I've read lately and my summary reaction.
<div class="note__hr"></div>

{% for book in site.books reversed %}
  <div class="note__date">{{ book.title }} - {{ book.author }}</div>
  <p>{{ book.content | markdownify }}</p>
  <span>[goodreads link]({{ book.link }})</span>
  <div class="note__hr"></div>
{% endfor %}