---
title: Categories
subtitle: Articles grouped by discipline.
permalink: /categories/
---
{% for category in site.categories %}
<section id="{{ category.first }}">
  <h2>{{ category.first | capitalize }}</h2>
  <div class="card-grid">
  {% for post in category.last %}
    {% include post-card.html post=post %}
  {% endfor %}
  </div>
</section>
{% endfor %}
