---
layout: archive
title: Articles
permalink: /articles/
excerpt: one step,one note
---
<div class="tiles">
{% for post in site.posts %}
	<p style="margin:5px">
		{{ post.date | date: "%m-%d-%Y" }}
		&nbsp;&nbsp;
		<a href="{{post.url}}">
		&nbsp;&nbsp;{{ post.title }}
		</a>
	</p>
{% endfor %}
</div><!-- /.tiles -->
