---
layout: default
title: C3 Admin's Posts
---
<ul class="list-group">
	{% for post in site.tags.c3admin %}
	<li class="list-group-item">
		{% include postlist.html post=post %}
	</li>
	{% endfor %}
</ul>
