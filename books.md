---
title: Books
subtitle: Curated reading across physics, mathematics, philosophy, literature, AI, history, and psychology.
permalink: /books/
---
{% for group in site.data.books %}
<section class="book-section">
  <h2>{{ group[0] | replace: "_", " " | capitalize }}</h2>
  <div class="card-grid">
  {% for book in group[1] %}
    <article class="post-card">
      <h3>{{ book.title }}</h3>
      <p><strong>{{ book.author }}</strong></p>
      <p>{{ book.summary }}</p>
      <p><strong>Difficulty:</strong> {{ book.difficulty }}</p>
      <p><strong>Recommended for:</strong> {{ book.recommended_for }}</p>
    </article>
  {% endfor %}
  </div>
</section>
{% endfor %}
