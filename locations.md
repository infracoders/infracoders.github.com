---
layout: default
title: "Locations"
permalink: /locations/index.html
location: Melbourne, Australia
---
<section class="container">
<div class="row">
<header class="span12">
<h2>Locations</h2>
</header>
</div> 
</section>

<section class="section-box locations shadow">
<div class="container">
<div class="row">
{% for post in site.categories.locations reversed %}
<article class="span4 center-align">
<a href="{{ post.link }}"><img src="http://maps.googleapis.com/maps/api/staticmap?center={{ post.location }}&amp;zoom=12&amp;size=350x150&amp;maptype=roadmap&amp;sensor=false" />
<h3>{{ post.location }}</h3></a>
</article>
{% endfor %}
</div>
</div>
</section>	

<section class="container">
<div class="row">
<header class="span12 center-align">
<h4>If you would like to start an InfrastructureCoders meetup in your city, please contact <a href="https://twitter.com/geekle">Matt</a> or <a href="https://twitter.com/dlutzy">David</a>.</h4>
</header>
</div>
</section>
