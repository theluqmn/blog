---
layout: index_updates
permalink: /updates
---

{% for post in site.categories.updates %}

## {{ post.date | date: "%d %B %Y" }}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
