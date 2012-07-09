---
layout: default
title: PeerDrive Blog
---

{% for post in site.categories.blog limit:3 %}
[{{ post.title }}]({{ post.url }})
==================================
<p class="meta">{{ post.date | date_to_string }}</p>

{{ post.content }}

{% endfor %}

{% if site.categories.blog.size > 3 %}

--------------------------------------------------------------------------

Older posts
===========

{% for post in site.categories.blog offset:3 %}
* {{ post.date | date_to_string }} -- [{{ post.title }}]({{ post.url }})
{% endfor %}

{% endif %}
