---
layout: minimal
title: Random Post
subtitle: Here is a page for random post, it is a work in progress. If you have any suggestions on how it can be improved please do get in touch.
---

{% assign random = site.time | date: "%s%N" | modulo: site.posts.size %}


{{ site.posts[random] }}
