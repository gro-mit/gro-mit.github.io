---
layout: archive
permalink: /thoughts/
title: "Thoughts"
excerpt: "Thoughts start from here"
---

<div class="tiles">
{% for post in site.posts %}
	{% if post.categories contains 'thoughts' %}
		{% include post-grid.html %}
	{% endif %}
{% endfor %}
</div><!-- /.tiles -->
