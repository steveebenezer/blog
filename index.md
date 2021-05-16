---
layout: default
title: "home"
---

{% for post in site.posts %}
  - <span><time>{{ post.date | date_to_string: "ordinal", "US" }}</time></span> -  [{{post.title}}]({{ post.url }})
{% endfor %}
