---
layout: index
section: reading
title: reading
description: "insights on the books i have read"
permalink: "/reading"
---

i am quite the bookworm, hence i decided to write posts summarising the books i read, as well as to share the main insights i got.

## books i have read

sorted according to date.

{% for post in site.categories.reading %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
