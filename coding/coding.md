---
layout: index
section: "coding blog"
title: coding blog
description: "my humble coding blog - where i share things related to software development, and coding/programming!"
permalink: "/coding"
---

a warm welcome to my humble coding blog - where i share things related to software development, and coding/programming! i hope you will be able to gain a new insight/knowledge or two from my posts :)

## posts

sorted according to date.

{% for post in site.categories.coding %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
