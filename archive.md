---
title: Archive
subtitle: All essays in chronological order.
permalink: /archive/
---
{% assign posts_by_year = site.posts | group_by_exp: "post", "post.date | date: '%Y'" %}
{% for year in posts_by_year %}
## {{ year.name }}
{% for post in year.items %}
- [{{ post.title }}]({{ post.url | relative_url }}) · {{ post.date | date: "%B %-d, %Y" }} · {{ post.categories | join: ", " }}
{% endfor %}
{% endfor %}

## Categories
{% for category in site.categories %}
- [{{ category[0] | capitalize }}]({{ '/categories/#' | append: category[0] | relative_url }}) ({{ category[1].size }})
{% endfor %}

## Tags
{% for tag in site.tags %}
- [{{ tag[0] }}]({{ '/tags/#' | append: tag[0] | relative_url }}) ({{ tag[1].size }})
{% endfor %}
