---
layout: page
title: Your Final Boss
tagline: If You Can Beat Him, You Can Beat Anything
---
{% include JB/setup %}

<div class="posts">
	{% for post in site.posts %}
		<div class="post">
				<img src="thumbnails/{{ post.topic-image }}" />
				<span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
				<span>{{ post.excerpt }} &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">Read more</a></span>
		</div>
	{% endfor %}
</div>
