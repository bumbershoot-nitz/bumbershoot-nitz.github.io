---
layout: photography
title: Photography
nav-menu: false
description: Photography goes here
image: assets/images/banner.png
permalink: "/photography.html"
---

<!-- Thumbnail -->
<section id="thumbnails">
{% for photo in site.photos %}
	<article>
		<a class="thumbnail" href="{{ photo.image }}" data-position="left center"><img src="{{ photo.thumbnail }}" alt="" /></a>
		<h2>{{ photo.title }}</h2>
		<p>{{ photo.caption }}</p>
	</article>
{% endfor %}
</section>
