---
layout: page
title: Notes
permalink: /notes/
---

Here are my posts:

{% if site.posts %}
	<ul class="post-list">
		{% for item in site.posts %}
			<li class="post-list__item">
				<article class="tease">
					<h3 class="tease__title">
						<a href="{{ item.url }}">
							{{ item.title }}
						</a>
					</h3>
				</article>
			</li>
		{% endfor %}
	</ul>
{% endif %}