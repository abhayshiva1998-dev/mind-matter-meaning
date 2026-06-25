---
title: Physics
subtitle: Physical law, measurement, matter, fields, thermodynamics, and spacetime.
permalink: /physics/
---
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'physics'" %}
<div class="card-grid">
{% for post in posts %}
  {% include post-card.html post=post %}
{% endfor %}
</div>
