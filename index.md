---
layout: index_all
---

All my posts!

{% for post in site.posts %}

## {{ post.date | date: "%d %B %Y" }}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.excerpt | markdownify | strip_html }}

{% endfor %}
