---
title: Role of Pediatric OT
image: /images/image-5.png
header: #
author: Missy
published: true
comments: true
categories: 
    - Readiness
    - Pediatrcis
    - Driving
layout: post
---

For teenagers, driving is a sort of rite of passage. It indicates transitioning into adulthood and offers a sense of freedom at various times throughout life. Driving usually starts out as fun or cool for most kids but quickly adds to their functional independence. Teens drive to extracurricular school events and work, to hang out with friends, or. 

<small>[more...](/docs/the-role-of-ot-in-driving-readiness-with-adolescents-most-at-risk.pdf)</small>

### Published Source
[TherapyFunZone.net - The Role of OT in Driving Readiness with Adolescents...](https://therapyfunzone.net/blog/the-roll-of-ot-in-driving-readiness-with-adolescents-most-at-risk/)


<!--### Screenshot Link to Published Page-->

![Teaching Readiness to Teens](/images/yunnan/yn8.jpg)


<section id="services">
	<div class="container">
		<div class="row">
			<div class="col-md-12">
<!--				<h3 class="section-title text-center rev">My Services</h3>-->
			</div>
		</div>
		<div class="row">
			{% for item in site.data.law %}
			<div class="col-md-4 col-sm-6">
				<a href="{{item.link}}">
					<div class="serviceBox cards rev">
						<div class="service-icon">
							<!-- <span><i class="fa {{item.fa-icon}}" aria-hidden="true"></i></span> -->
							<img src="">
						</div>
						<h3 class="title">{{item.title}}</h3>
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
