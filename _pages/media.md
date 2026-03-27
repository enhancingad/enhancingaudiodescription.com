---
layout: page
title: Media
permalink: /media/
image: 
---

<head>
<style>
.page__info {
  max-width: 1024px;
  }
.page {
  max-width: 1024px;
}
</style>
</head>

<div class="container">
  <h2>Selected Video</h2>
  <h3>EAD Spotlight</h3>
  <p>The EAD Spotlight by Mariana and Gavin delivered as part of the DARCI Conference in September 2025 (University of York), outlining what the methods are, the work done in collaboration with filmmakers and future steps. 
Descriptions are integrated to the talk and the examples of EAD are best experienced over headphones.</p>
    <article class="post">
    <div class="post__content">
    <iframe title="vimeo-player" src="https://player.vimeo.com/video/1162539907?h=e703c41a48" width="640" height="360" frameborder="0" referrerpolicy="strict-origin-when-cross-origin" allow="autoplay; fullscreen; picture-in-picture; clipboard-write; encrypted-media; web-share"   allowfullscreen></iframe></div>
    </article>
  <h2>All Videos</h2>
  <p>This section contains a list of blog posts featuring our videos. The videos are best experienced over headphones.</p>

  <div class="row animate">
    {% if site.posts.size > 0 %}
      {% for post in site.posts %}
        {% if post.tags contains "video" %}
        {% if post.grid != false %}
        {% include article.html %}
        {% endif %}
        {% endif %}
      {% endfor %}
    {% endif %}
  </div>
<h2>Podcasts</h2>
  <div class="row animate">
    {% if site.posts.size > 0 %}
      {% for post in site.posts %}
        {% if post.tags contains "podcast" %}
        {% if post.grid != false %}
        {% include article.html %}
        {% endif %}
        {% endif %}
      {% endfor %}
    {% endif %}
    <!-- <p>Our podcast can also be enjoyed via our playlist on our <a href="https://soundcloud.com/user-351945045">Soundcloud account</a>.</p>-->
  </div>
</div>