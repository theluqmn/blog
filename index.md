---
layout: index_all
---

{% for post in site.posts %}

## {{ post.date }}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
