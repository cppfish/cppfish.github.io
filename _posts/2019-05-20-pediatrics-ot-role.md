---
title: Role of Pediatric OT
image: #
header: #
author: Luke
published: true
comments: true
categories: 
    - Readiness
layout: post
---


<section id="services">
	<div class="container">
		<div class="row">
			{% for item in site.data.law %}
			<div class="col-md-3 col-sm-6">
				<a href="{{item.link}}"  target="_blank">
					<div class="serviceBox cards rev">
						{{item.title}}
					</div>
				</a>
			</div>
			{% endfor %}
		</div>
	</div>
</section>

<!-- <div>
	<img src="{{item.image}}">
</div>

<p class="description">
{{item.description}}
</p> -->