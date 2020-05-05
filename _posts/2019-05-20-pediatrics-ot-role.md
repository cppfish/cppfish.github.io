---
title: Role of Pediatric OT
image: #
header: #
author: Luke
published: true
comments: true
categories: 
    - Readiness
    - Pediatrcis
    - Driving
layout: post
---

For teenagers, driving is a sort of rite of passage. It indicates transitioning into adulthood and offers a sense of freedom at various times throughout life. Driving usually starts out as fun or cool for most kids but quickly adds to their functional independence. Teens drive to extracurricular school events and work, to hang out with friends, or. 


### Published Source




### My Services 

<section id="services">
	<div class="container">

		<div class="row">
			{% for item in site.data.law %}
			<div class="col-md-3 col-sm-6">
				<a href="{{item.link}}">
					<div class="serviceBox cards rev">
						<div>
							<img src="{{item.image}}">
						</div>
						{{item.title}}
						<p class="description">
							{{item.description}}
						</p>

					</div>
				</a>
			</div>

			{% endfor %}
		</div>
	</div>
</section>
