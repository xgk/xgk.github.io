---
layout: page
title: XGeek's Technical Blog
tagline: Cloud Computing
---
{% include JB/setup %}

<ul class="posts">
{% for post in site.posts %}
	<li>
		<h3 class="title">
		<span>{{ post.date | date_to_string }}</span>
		&raquo; 
		<a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
		</h3>
		<hr>
		<article> {{ post.excerpt | strip_html}} </article>
		<a href="{{ BASE_PATH }}{{ post.url }}">Read more...</a>
	</li>
	<hr>
{% endfor %}
</ul>


