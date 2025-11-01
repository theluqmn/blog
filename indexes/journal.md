---
layout: index_journal
permalink: /journal
---

{% for post in site.categories.journal %}

## {{ post.date | date: "%d %B %Y" }}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
