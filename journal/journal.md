---
layout: index
section: "luqman's journal"
description: "my personal journal, where i write about things that has happened in my life."
permalink: "/journal"
---

# journal

welcome to my personal journal, where i write about things that has happened in my life - projects, events, competitions, updates, and more!

## journal entries

sorted according to date.

{% for post in site.categories.journal %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
