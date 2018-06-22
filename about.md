---
layout: page
title: About
permalink: /about/
---

<br>
<div class="grid-container">
<div class="grid-60">


<h4>Hello! I'm Jordan.</h4>
{% capture my_bio %}{% include bio.md %}{% endcapture %}
{{ my_bio | markdownify }}

<ul class="sociallinks footersocial">
<b>Want to get in touch?</b>
<a href="mailto:{{site.email}}"><li><i class="fa fa-envelope"></i> Say Hello</li></a>
</ul>


</div>
<div class="grid-40">
<br>
<div class="grid-container achievecontain">
<a class="linkedintext" href="//linkedin.com/in/jordanshuck"><div class="linkedin">
Visit me on <i class="fa fa-linkedin-square" aria-hidden="true"></i>
</div></a><br>

<b>Experience:</b>
<br><br>

{% for post in site.categories.achievement | sort: 'date') | reverse %}
<div class="achievebox" style="background:rgba{{ post.uniquecolour }}; ">
<img class="achieveimg" src="{{ site.baseurl }}/images/{{ post.symbol }}">
<p class="achievebold">{{ post.title }}</p>
<span class="bottominfo">
<p class="briefskills">{{ post.level }}</p>
<p class="achievewhen">{{ post.bottom }}</p>
</span>
</div>

{% endfor %}
</div>

<style>
.post-title {
	display: none;
}

