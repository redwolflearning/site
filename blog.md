---
layout: page
title: Blog
permalink: /blog/
---

{% for post in site.posts %}

<div class="blog-card">
<span class="post-meta">{{ post.date | date: "%B %d, %Y" }}</span>
<h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
<p>{{ post.description }}</p>
<p><a href="{{ post.url | relative_url }}">Read the post</a></p>
</div>

{% endfor %}
