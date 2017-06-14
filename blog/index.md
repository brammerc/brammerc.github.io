---
title: Blog
layout: page
---

# Sport Performance Analytics
<!--Exploratory data analysis (letter values, boxplots, letter value boxplots, density plots, stem-and-leaf, QQ plots...Re-expression, robust-resistant linear fit to bivariate data, G&H, Smoothing (spline, lowess)), Time series analysis (smoothing techniques, fouier (cos simulation), ARMA, ARIMA, ARIMAX, VARIMAX), Multivariate anlysis (matrix algebra, MANOVA, cluster analysis, scree plot, factor analysis, multiple regression, linear mixed effect models)  --> 

#### This blog attempts to describe, in plain language, various methods used to process, visualize, and analyze human performance data.

<hr/>

<div id="posts">

    {% for post in site.posts offset: 0 limit: 10 %}
    	<h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
	    <h5>{{ post.date | date: "%B %d, %Y" }}</h5>
	    {% if post.image %}
	    <p>
	    	<a href="{{ post.url }}"><img class="centered" src="/images/blog/{{post.image}}" alt=""></a>
    	</p>
    	{% endif %}
        <p>{{ post.excerpt }} </p>
        <p>	<a class="graybutton" href="{{ post.url }}">Read more</a></p>
        <hr/>
    {% endfor %}

	<p>
	<a class="greenbutton" href="/blog/archive/" title="an archive of all posts">See all posts &rarr;</a>
	</p>
	
</div>