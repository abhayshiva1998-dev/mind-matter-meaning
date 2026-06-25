---
title: Philosophy
subtitle: Metaphysics, epistemology, logic, ethics, and the analysis of concepts.
permalink: /philosophy/
---
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'philosophy'" %}
<div class="card-grid">
{% for post in posts %}
  {% include post-card.html post=post %}
{% endfor %}
</div>
