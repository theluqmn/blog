---
layout: index_coding
permalink: /coding
---

{% for post in site.categories.coding %}

## {{ post.date | date: "%d %B %Y" }}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
