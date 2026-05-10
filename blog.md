---
layout: page
title: Blog
permalink: /blog/
---

# Blog

{% raw %}{% for post in site.posts %}{% endraw %}

## [{{ post.title }}]({{ post.url }})

*{{ post.date | date: "%B %d, %Y" }}*

{{ post.excerpt }}

{% raw %}{% endfor %}{% endraw %}
