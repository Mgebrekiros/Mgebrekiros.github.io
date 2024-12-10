---
layout: default
title: "Archives"
permalink: /archives/
---

# Blog Archives

{% for post in site.posts %}
  <p>{{ post.date | date_to_string }} » <a href="{{ post.url }}">{{ post.title }}</a></p>
{% endfor%}
