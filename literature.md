---
title: Literature
subtitle: Form, interpretation, criticism, memory, and human experience.
permalink: /literature/
---
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'literature'" %}
<div class="card-grid">
{% for post in posts %}
  {% include post-card.html post=post %}
{% endfor %}
</div>
