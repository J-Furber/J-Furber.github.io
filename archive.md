---
layout: page
title: Blog
---
The posts done here more focus on the first two years (with a bit for my third year). Evidently I started to focus more of my writing time into my thesis rather than into blog posts by the end of the PhD! I don't think I will be adding some any time soon.

{% for tag in site.tags %}
<h3>{{- tag[0] -}}</h3>
<ul>
  {%- for post in tag[1] %}
  <li><a href="{{ post.url }}">{{ post.date | date: "%b %Y" }} - {{ post.title }}</a></li>
  {%- endfor %}
</ul>
{%- endfor %}
