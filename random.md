---
layout: post
title: 
---

{% assign random = site.time | date: "%s%N" | modulo: site.posts.size %}

<blockquote>&ldquo;{{ site.posts.size[random].quote }}&rdquo; <cite>{{ site.data.inspirational-quotes[random].person }}</cite></blockquote>
<h1>{{ site.posts[random].title }}</h1>

<ul class="content">
{% for post in site.posts %}
  <li class="listing">
    <hr class="slender">
    <a href="{{ post.url }}"><h4 class="contrast">{{ post.title }}</h4></a>
    <span class="smaller">{{ post.date | date: "%B %-d, %Y" }}</span>  <br/>
    <div>{{ post.excerpt }}</div>

  </li>
{% endfor %}
