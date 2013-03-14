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
{% for post in site.categories.locations reversed %}
{% capture thecycle %}{% cycle 'odd', 'even' %}{% endcapture %}
<div class="row">
{% if thecycle == 'odd' %}
<div class="span4"><img src="http://maps.googleapis.com/maps/api/staticmap?center={{ post.location }}&zoom=12&size=350x150&maptype=roadmap&sensor=false" /></div>
<div class="span8 vertical-align-middle"><h3><a href="{{ post.permalink }}">{{ post.location }}</a></h3></div>
{% else %}
<div class="span8"><h3><a href="{{ post.permalink }}">{{ post.location }}</a></h3></div>
<div class="span4 pull-right"><img src="http://maps.googleapis.com/maps/api/staticmap?center={{ post.location }}&zoom=12&size=350x150&maptype=roadmap&sensor=false" /></div>
{% endif %}
</div>
{% endfor %}
</div>
</section>	

<section class="container">
<div class="row">
<header class="span12 pagination-centered">
<h4>If you would like to add an event please submit a pull request. <a href="https://github.com/infracoders/infracoders.github.com" target="_blank">https://github.com/infracoders/infracoders.github.com</a></h4>
</header>
</div>
</section>
