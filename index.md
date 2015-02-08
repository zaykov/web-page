---
layout: page
title: Latest Posts
excerpt: "Pavel G. Zaykov personal home page."
tags: [Pavel Zaykov, Pavel G. Zaykov home page, personal blog, projects, dowloads, publications]
search_omit: true
image:
  feature: aero-1.jpg
  credit: Honeywell
  creditlink: http://aerospace.honeywell.com/
---

<ul class="post-list">
{% for post in site.posts limit:5 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

