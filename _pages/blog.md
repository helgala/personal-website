---
layout: page
title: blog
permalink: /blog/
nav: false
description: Research and academic updates from Hany Elgala.
---

Selected updates about research and academic work. Each post links to the original university announcement.

{% assign sorted_posts = site.posts | sort: 'date' | reverse %}
{% for post in sorted_posts %}

### [{{ post.title }}]({{ post.url | relative_url }})

{{ post.date | date: '%B %-d, %Y' }} · {{ post.description }}

{% endfor %}
