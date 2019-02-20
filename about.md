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

Latest Radio Show:
<iframe width="100%" height="120" src="https://www.mixcloud.com/widget/iframe/?hide_cover=1&light=1&feed=%2FShockRadio%2Fbreakfast-with-jonty-and-jordan-19022019%2F" frameborder="0" ></iframe>

<a class="twitter-timeline" data-width="400" data-height="500" href="https://twitter.com/jshuckie?ref_src=twsrc%5Etfw">Tweets by jshuckie</a> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
