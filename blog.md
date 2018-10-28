---
layout: page
title: Blog
permalink: /blog/
---

{% for post in site.posts %}
{% if post.categories contains 'blog' or post.categories contains 'university' %}
  <article class="post-preview">
  <div class="featuredImage" style="background-image: url({{site.baseurl}}/images/blog/{{post.featuredImage}});"></div>
  <a class="blogdesc" href="{{ post.url | prepend: site.baseurl | replace: '//', '/' }}">
  <div class="blogpost">
      <h2 class="post-title">{{ post.title }}</h2>
      {% if post.shortdesc %}
      <span class="pagedesc">{{ post.shortdesc | strip_html | truncatewords: 40 }}</span><br>
      {% endif %}
    <br>
    <p class="post-meta">Posted
      {% if post.shortdesc %}
        under <span class="categorylink">{{ post.categories }}</span>
      {% endif %}
      {% if post.author %}
        {{ post.author }}
      {% else %}
        {{ site.author }}
      {% endif %}
      on {{ post.date | date: '%B %d, %Y' }}</p>

  </div></a></article>
{% endif %}

{% endfor %}

<!-- Pager -->
{% if paginator.total_pages > 1 %}

  <div class="clearfix">

    {% if paginator.previous_page %}
      <a class="btn btn-primary float-left" href="{{ paginator.previous_page_path | prepend: site.baseurl | replace: '//', '/' }}">&larr; Newer<span class="d-none d-md-inline"> Posts</span></a>
    {% endif %}

    {% if paginator.next_page %}
      <a class="btn btn-primary float-right" href="{{ paginator.next_page_path | prepend: site.baseurl | replace: '//', '/' }}">Older<span class="d-none d-md-inline"> Posts</span> &rarr;</a>
    {% endif %}

  </div>

{% endif %}

<style>
.pagedesc a{
  font-size: 18px !important;
  text-decoration: none !important;
}
.pagedesc:hover {
  text-decoration: none !important;
}
.featuredImage {
  width: 150px;
  height: 150px;
  background-size: cover;
  background-position: center;
  float: right;
  margin-top: 20px;
  margin-left: 20px;
}

.post-preview {
  margin-top: 40px;
  border-top: 1px solid #eee;
  padding: 30px;
}
.blogpost:hover .post-title {
  text-decoration: underline !important;
}


.blogdesc:hover {
  text-decoration: none;
}
</style>
