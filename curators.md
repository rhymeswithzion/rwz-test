---
layout: page
title: Curators
---

Here are a list of curators who regularly contribute to the website:

<ul>
  {% for author in site.authors %}
    <li><a href="{{ author.url }}">{{ author.title }}</a></li>
  {% endfor %}
</ul>

If you are interested in becoming a curator, please follow the instructions on the <a href="https://docs.google.com/document/d/1u7PoI3MD21fb0GxSsZyfxVKJhmEE8eP3cbyBOWyufss" target="_blank">curators template</a>. 
