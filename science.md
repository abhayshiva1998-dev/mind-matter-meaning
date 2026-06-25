---
title: Science
subtitle: Evidence, explanation, method, and the history of scientific change.
permalink: /science/
---
{% assign posts = site.posts | where_exp: "post", "post.categories contains 'science'" %}
<div class="card-grid">
{% for post in posts %}
  {% include post-card.html post=post %}
{% endfor %}
</div>
