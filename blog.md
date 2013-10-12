---
layout: default
title: C3 Blog
---
<ul class="list-group">
	{% for post in site.posts %}
	<li class="list-group-item">
		<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
		{% assign num_words = post.content | number_of_words %}
		<p>
			Posted on {{ post.date | date_to_long_string }} by <a href="/author/{{ post.tags }}">{{ post.tags | array_to_sentence_string }}</a>, {{ num_words }} {% if num_words == 1 %}word{% else %}words{% endif %}
		</p>
		{% assign category_sentence = post.categories | array_to_sentence_string %}
		{% if category_sentence != '' %}
		<p>Categories: {{ category_sentence }}</p>
		{% endif %}
		<blockquote>
		<p>{{ post.excerpt }}</p>
		</blockquote>
	</li>
	{% endfor %}
</ul>
