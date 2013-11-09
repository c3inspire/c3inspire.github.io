---
layout: default
title: About the Team
---
## Want to be part of the Team?
We're constantly looking for talented individuals to join the team. If you're interested in helping out, please contact us. We also have various positions available on the Exec Team, find the one that suits you and apply to be part of the Team!

**We're now looking for University Team Leads,** who will assist the Executive Team in creating the Conference and driving awareness among their fellow students. The Team Leads will get an opportunity to work on a National Conference, and will also get to network with prominent Industry Professionals to gain valuable insight into successful Entrepreneurship.

## The Executive Team

<ul class="media-list">
	{% for member in site.data.team %}
	<li class="media">
		<img class="media-object pull-left" src="{{ member.photo }}" alt="{{ member.name }}">
		<div class="media-body">
			<h4 class="media-heading">{{ member.name }}, {{ member.title }}</h4>
			<p>{{ member.bio }}</p>
		</div>
	</li>
	{% endfor %}
</ul>
