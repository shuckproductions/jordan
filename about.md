---
layout: page
title: About
permalink: /about/
---
<style>
@import url('http://productions.shuck.org.uk/grid.css');

.grid-10 {
width: 10% !important;
}

.grid-achievemini {
height: 140px !important;
}
/**** About page styles ***/
.achievebox { padding: 10px; height: 170px; text-align: center; color: #fff; margin-right: 10px; padding: 15px; display: block; min-width: 125px; position: relative; margin-bottom: 20px; }

.achieveimg { margin-left: auto; margin-right: auto; max-height: 50px !important; min-width: 10px !important; margin-bottom: 6px !important; background-repeat: no-repeat !important; display: block; float: none !important; padding: 0px !important; width: 50px !important; margin-bottom: 20px !important; }

.achievebold { font-weight: 500; font-size: 18; line-height: 1 !important; }

.achievelevel { font-weight: 300; font-size: 15px; margin-bottom: 0px !important; padding-bottom: 10px; }

.briefskills { font-weight: 400; font-size: 12px; line-height: 1.3 !important; }

.achievewhen { font-size: 12px; line-height: 0.2; padding-top: 5px; padding-bottom: 5px; }

.bottominfo { bottom: 0; margin-bottom: 0px !important; position: absolute; width: 80%; left: 0; width: 100%; }

.grid-achieve { margin-right: 70px; }</style>


Hi! I’m Jordan. I’m 18 from Blackpool, Lancashire. I’m an aspiring producer/director/actor. I currently attend Baines Sixth form, in upper sixth, where I am studying Biology, ICT and Media Studies. 

I trained at Scream Theatre Schools in all three disciplines. Also I am an active member of Blackpool Scouts where I am Deputy Youth Commissioner, an assistant Beaver leader at 1st Bispham Scout and Guide Group, a part of the production team for Blackpool Gang Show and the Media & Communications Editor for the Blackpool District. 

Most recently have started making short films and promotional materials for myself and others, under  Shuck Productions. If you want to view my films/videos please look at the 'Productions' section on my site.

**Television Credits:**

<div class="grid-container">
{% for post in site.categories.tv | sort: 'date') | reverse %}
<div class="grid-10 mobile-grid-100 grid-achieve">
<div class="achievebox  grid-achievemini" style="color:rgba{{ post.uniquecolour }}!important; background-color:#F1F1F1; ">
<img class="achieveimg" src="{{ site.baseurl }}/images/{{ post.symbol }}">
<p class="achievebold">{{ post.title }}</p>
<span class="bottominfo">
<p class="briefskills">{{ post.level }}</p>
<p class="achievewhen">{{ post.bottom }}</p>
</span>
</div></div>
{% endfor %}

</div>

**Theatre:**

<div class="grid-container">
{% for post in site.categories.theatre | sort: 'date') | reverse %}
<div class="grid-10 mobile-grid-100 grid-achieve">
<div class="achievebox  grid-achievemini" style="color:rgba{{ post.uniquecolour }}!important; background-color:#F1F1F1; ">
<img class="achieveimg" src="{{ site.baseurl }}/images/{{ post.symbol }}">
<p class="achievebold">{{ post.title }}</p>
<span class="bottominfo">
<p class="briefskills">{{ post.level }}</p>
<p class="achievewhen">{{ post.bottom }}</p>
</span>
</div></div>
{% endfor %}

</div>

**Achievements:**

<div class="grid-container">

{% for post in site.categories.achievement | sort: 'date') | reverse %}
<div class="grid-10 mobile-grid-100 grid-achieve">
<div class="achievebox" style="background:rgba{{ post.uniquecolour }}; ">
<img class="achieveimg" src="{{ site.baseurl }}/images/{{ post.symbol }}">
<p class="achievebold">{{ post.title }}</p>
<span class="bottominfo">
<p class="briefskills">{{ post.level }}</p>
<p class="achievewhen">{{ post.bottom }}</p>
</span>
</div></div>

{% endfor %}
</div>


<ul class="sociallinks footersocial">
<b>Contact me:</b>
<a href="mailto:{{site.email}}"><li><i class="fa fa-envelope"></i></li></a>
</ul>
