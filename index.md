---
layout: index
---

# hello there

**blog.theluqmn.com** is my personal blog where i share what i think deserves to be on the internet. typically consists of life updates, thoughts, some technical stuff and random things. if you are interested in leadership, entrepreneurship, tech, and cool stuff, check out my newsletter [the revelations](https://revelations.theluqmn.com).

## how this works

this is a relatively simple and straightforward static site, built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/). i write my posts in markdown then GitHub builds the site for me when it detects a change in the repository.

i chose to use jekyll because it gets the job done quite well and i don't have to worry about hosting the site myself. additionally, its simple and allows me to focus on writing. i highly recommend using jekyll if you want to build a simple blog. oh btw, you can customise the theme/layout to your liking using HTML. the layout im using is custom-made by me.

## all posts

{% for post in site.posts %}

### [{{ post.title }}]({{ post.url | relative_url }})

**{{ post.date | date: "%d %B %Y" }}** - {{ post.excerpt | markdownify | strip_html }}

{% endfor %}
