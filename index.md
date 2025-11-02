---
layout: index_all
permalink: /
---

{% for post in site.posts %}

## {{ post.date | date: "%d %B %Y" }}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.categories[0] }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
