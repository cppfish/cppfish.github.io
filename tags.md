---
title: "标签"
layout: Tags
permalink: /tags
---

<!-- reference https://github.com/luolinjia/cn/tree/gh-pages -->


<div id='tag_cloud'>
{% for tag in site.tags %}
<a href="#{{ tag[0] }}" title="{{ tag[0] }}" rel="{{ tag[1].size }}">{{ tag[0] }}</a>
{% endfor %}
</div>

<div class = "episodes">

<ul class="listing">
{% for tag in site.tags %}
  <li class="listing-seperator {{ tag[0] }}">{{ tag[0] }}</li>
{% for post in tag[1] %}
  <li class="listing-item {{ tag[0] }}">
  
   {% comment %}
  <time datetime="{{ post.date | date:"%Y-%m-%d" }}">{{ post.date | date:"%Y-%m-%d" }}</time>
   {% endcomment %}
  
  <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}" class="listing-item-a">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>
</div>


<script language="javascript">
    $.fn.tagcloud.defaults = {
        size: {start: 14, end: 96, unit: 'px'},
        color: {start: '#ACE6E6', end: '#226666'}
    };
    $(function () {
        $('.listing-seperator, .listing-item').hide();
        var recentColor, recentSize;
        $('#tag_cloud a')
            .tagcloud()
            .mouseover(function(){
                var thiz = $(this);
                recentColor = thiz.css('color');
                //recentSize = thiz.css('font-size');
                thiz.css({'color': '#226666'});
            })
            .mouseout(function(){
                $(this).css({'color': recentColor});
            })
            .click(function() { // update the showing tags style
                var clazz = $(this).html();
                $('.listing-seperator, .listing-item').hide();
                $('.' + clazz).show();
            });
    });
</script>
