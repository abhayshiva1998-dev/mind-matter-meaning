---
title: Categories
subtitle: Articles grouped by discipline.
permalink: /categories/
---
{% for category in site.categories %}
<section id="{{ category[0] }}">
  <h2>{{ category[0] | capitalize }}</h2>
  <div class="card-grid">
  {% for post in category[1] %}
    {% include post-card.html post=post %}
  {% endfor %}
  </div>
</section>
{% endfor %}
