---
layout: default
title: "Geeky Giveaway Challenge"
permalink: /giveawaychallenge.html
---
<section class="container">
<div class="row">
<header class="highlight span12">
<h2>Geeky Giveaway Challenge</h2>
</header>
</div> 
</section>

<section class="container">
<div class="row">
We often have things to give away out our meetups.  T-Shirts, stickers, tech books. But how to choose the winner(s)?  

Here's the geeky giveaway challenge. Come up with the most pointlessly elaborate way of picking the winner of the giveway.  You'll have 5 minutes to demonstrate the method and will win the admiration of your peers.

</div>
<div class="span12 "><hr></div>
</section>

<section class="container">
{% for hack in site.categories.giveaways %}
<div class="span12 "><b>Author:</b> {{ hack.author }} 
{% if hack.link != null %} <a href="http://twitter.com/{{hack.twitter}}">http://twitter.com/{{hack.twitter}}</a>
{% endif %}
</div>
<div class="span12 "><b>Title:</b> {{ hack.title }}</div>
{% if hack.link != null %} 
    <div class="span12"><b>Link:</b> <a href="{{ hack.link }}" target="_blank">{{ hack.link}}</a> </div>
{% endif %}
{% if hack.source != null %} 
    <div class="span12"><b>Source Code:</b> <a href="{{ hack.source }}" target="_blank">{{ hack.source }}</a> </div>
{% endif %}
<div class="span12"><b>Description:</b> {{ hack.description }}</div>
<div class="span12"><b>Bugs?</b> {{ hack.bugs }}</div>
<div class="span12 "><hr></div>
{% endfor %}
</section>	

<section class="container">
<div class="row">
<header class="span12 offset2">
</header>
</div>
</section>
