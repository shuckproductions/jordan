---
layout: page
title: Performances
permalink: /performances/
---

A gallery of some of my performances...
<br><br>
<hr class="line">
<br>
<center>
{% for post in site.categories.performance %}
<div class="performancepost">
<h4 class="gallerytitle">{{ post.title }} </h4>
<span class="performancedate">{{ post.date | date: '%B, %Y' }}</span><br><br>
{{ post.content }}
<hr class="line">
</div>
{% endfor %}
</center>