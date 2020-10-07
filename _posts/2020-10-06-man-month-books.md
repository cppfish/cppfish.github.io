---
title: 人月神话
image: /images/image-5.png
header: #
author: john
published: true
categories: 
    - work
layout: post
---


人月神话

人生三大错觉：

- 手机在响
- 她喜欢我
- 我能反杀


<section id="books">
	<div class="container">
		<div class="row">
			<div class="col-md-12">
			</div>
		</div>
		<div class="row">


{% for item in site.data.books %}
<div class="col-md-4 col-sm-6">
	<a href="{{item.link}}">
		<div class="serviceBox cards rev">
			<img src="{{item.image}}">
			<h3> {{item.title}} </h3>
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
