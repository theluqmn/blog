---
layout: index
permalink: "/journal"
---

# journal

welcome to my personal journal, where i write about things that is happening to my life at the moment - my life projects, updates, etc.

## journal entries

{% for post in category.posts %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
