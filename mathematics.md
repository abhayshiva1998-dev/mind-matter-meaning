---
title: Mathematics
subtitle: Proof, abstraction, logic, statistics, linear algebra, and structure.
permalink: /mathematics/
---
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'mathematics'" %}
<div class="card-grid">
{% for post in posts %}
  {% include post-card.html post=post %}
{% endfor %}
</div>
