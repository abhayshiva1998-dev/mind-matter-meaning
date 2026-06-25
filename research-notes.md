---
title: Research Notes
subtitle: Short notes, bibliographies, calculations, figures, and open questions.
permalink: /research-notes/
---
<div class="card-grid">
{% for note in site.research_notes %}
  {% include post-card.html post=note %}
{% else %}
  <p>No research notes have been published yet.</p>
{% endfor %}
</div>
