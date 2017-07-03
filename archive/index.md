---
layout: page
title: Archive
---

<div class="archive-list">
	<h1>Blog Archive</h1>
	<section class="listing">

   {% for post in site.posts %}
       {% assign currentDate = post.date | date: "%Y" %}
       {% if currentDate != myDate %}
           {% unless forloop.first %}</ul>{% endunless %}
           <b>{{ currentDate }}</b>
           <ul>
           {% assign myDate = currentDate %}
       {% endif %}
       <li><span>{{ post.date | date: "%B %-d, %Y" }}</span><a href="{{ post.url }}"> - {{ post.title }}</a></li>
       {% if forloop.last %}</ul>{% endif %}
   {% endfor %}
   
   </section>
</div>   

<hr>

<div id='tag_cloud'>
{% for tag in site.tags %}
<a href="#{{ tag | first | slugize }}/" title="{{ tag | first }}" style="font-size: {{ tag | last | size | times: 100 | divided_by: site.tags.size | plus:70 }}%">{{ tag | first }} ({{ tag[1].size }}) </a>
{% endfor %}
</div>

<p></p>

<ul class="listing">
{% for tag in site.tags %}
  <b class="listing-seperator" id="{{ tag[0] }}">{{ tag[0] }}</b>
{% for post in tag[1] %}
  <li class="listing-item">
  <time datetime="{{ post.date | date: "%m-%d-%Y" }}">{{ post.date | date: "%m-%d-%Y" }}</time>
  <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>

<!---
<div class="archive-list">
	<h1>Sport Performance Analytics</h1>
	<ul class="listing">
		{% for post in site.posts %}
		<li class="listing-item">
		  <time datetime="{{ post.date | date: "%m-%d-%Y" }}">{{ post.date | date: "%m-%d-%Y" }}</time>
		  <a href="{{ post.url }}" class="title">{{ post.title }}</a>
		</li>
		{% endfor %}
	</ul>
</div>

## Categories
<div id='tag_cloud'>
{% for cat in site.categories %}
<a href="#{{ cat[0] }}" title="{{ cat[0] }}" rel="{{ cat[1].size }}">{{ cat[0] }} ({{ cat[1].size }})</a>
{% endfor %}
</div>

<ul class="listing">
{% for cat in site.categories %}
  <li class="listing-seperator" id="{{ cat[0] }}">{{ cat[0] }}</li>
{% for post in cat[1] %}
  <li class="listing-item">
  <time datetime="{{ post.date | date: "%m-%d-%Y" }}">{{ post.date | date: "%m-%d-%Y" }}</time>
  <a href="{{ site.url }}{{ post.url }}" title="{{ post.title }}">{{ post.title }}</a>
  </li>
{% endfor %}
{% endfor %}
</ul>

<script src="/media/js/jquery.tagcloud.js" type="text/javascript" charset="utf-8"></script> 
<script language="javascript">
$.fn.tagcloud.defaults = {
    size: {start: 1, end: 1, unit: 'em'},
      color: {start: '#f8e0e6', end: '#ff3333'}
};

$(function () {
    $('#tag_cloud a').tagcloud();
});
</script>
--->
