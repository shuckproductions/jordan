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


Hello! I'm Jordan. I'm 18, have a love of broadcasting and I'm studying BA (Hons) Television and Radio at the University of Salford based at MediaCityUK.

One aspect of my course is to analyse a variety of content. On this blog, I am posting viewing and listening logs, where I analyse an array of content from broadcast to online. <a href="/blog/"> Have a gander! </a>

Blackpool born and bred. Who doesn't love the going up the tower, riding the Big One, seeing the illuminations and a little stick of Blackpool rock? (cue George Formby)

I am a producer at Shock Radio, Manchester's biggest student radio station. Why not tune in at <a href="shockradio.co.uk"> shockradio.co.uk. </a>

At A-level, I studied Biology, Media Studies and Information Technology (and Chemistry at AS). I also undertook an AQA extended project where I created a promotional video for Baines School following their brief and following the process from pre to post production.

Original broadcast television is where my love of the media lies; more specifically British TV fictions such as: Fawlty Towers, Doctor Who, Steptoe and Son, Allo Allo and much more...

I have trained in singing, acting and dancing at Scream Theatre Schools and I am managed by Scream Management (The Greenhouse, MediaCityUK). I have both on-screen and on stage credits, view them below.

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

Also, I am an active member of Blackpool Scouts where I am District Youth Commissioner, an assistant Beaver Scout leader, a producer for Blackpool Gang Show and Media and Communications Editor for Blackpool District. In all of these roles, I act as an ambassador for Blackpool Scouts and empower the young people to make their own decisions and be involved in shaping their scouting adventures.

I feel that I have a responsibility to entertain, inspire and engage with an audience; and this sparks my passion for the media, making me determined, focused and enthusiastic about all aspects of media production from writing to editing. I believe film, television and radio are the most important ways to tell a story and use creativity to form relationships with characters you have created to change people's opinions.

Broadcasting is one of the most powerful and influential tools that we have in society and I would love to be a part of the community that makes it happen. My goal is to be a producer or perhaps a director and I believe that through hard work and getting my degree will provide me with a stepping stone to help me achieve this goal.

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
