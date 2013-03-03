---
layout: default
title: "Events"
permalink: /events/index.html
---
<section class="container">
<div class="row">
<header class="highlight span12">
<h2>Infrastructure as code related events <strong>2013</strong></h2>
</header>
</div> 
</section>

<section class="container">
{% for post in site.categories.events reversed %}
<div class="span2 ">{{ post.date | date: "%B %e, %Y" }}</div>
<div class="span6"> <a href="{{ post.link }}" target="_blank">{{ post.title }}</a> </div>
<div class="span3">{{ post.location }}</div>
{% endfor %}
</section>	

<section class="container">
<div class="row">
<header class="span12 offset2">
<h4>If you would like to add an event please submit a pull request. <a href="https://github.com/infracoders/infracoders.github.com" target="_blank">https://github.com/infracoders/infracoders.github.com</a></h4>
</header>
</div>
</section>
