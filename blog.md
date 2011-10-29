---
layout: default
title: PeerDrive Blog
---

{% for post in site.posts limit:3 %}
[{{ post.title }}]({{ post.url }})
==================================
<p class="meta">{{ post.date | date_to_string }}</p>

{{ post.content }}

{% endfor %}

{% if site.posts.size > 3 %}

--------------------------------------------------------------------------

Older posts
===========

{% for post in site.posts offset:3 %}
* {{ post.date | date_to_string }} -- [{{ post.title }}]({{ post.url }})
{% endfor %}

{% endif %}
