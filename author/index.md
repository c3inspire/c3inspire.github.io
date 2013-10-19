---
layout: default
title: Authors
---
<ul class="list-group">
	{% for tag in site.tags %}
	<li class="list-group-item">
		{% if tag[0] == 'c3admin' %}
		<a href="/author/{{ tag[0] }}">C3 Admin's Posts</a><span class="badge">{{ tag[1].size }}</span>
		{% elsif tag[0] == 'tchen' %}
		<a href="/author/{{ tag[0] }}">Tony Chen's Posts</a><span class="badge">{{ tag[1].size }}</span>
		{% else %}
		<a href="/author/{{ tag[0] }}">Other Posts</a>
		{% endif %}
	</li>
	{% endfor %}
</ul>
