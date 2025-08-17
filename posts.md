---
layout: index
section: "posts"
description: "all the posts in blog.theluqmn.com"
permalink: "/posts"
---

# all posts

as requested, below is all the posts in this blog, in its corresponding categories.

{% for tag in site.tags %}

## {{ tag[0] }}

{% for post in tag[1] %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}

{% endfor %}
