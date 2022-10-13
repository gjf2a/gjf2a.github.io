---
layout: default
---

# Easy Assignments 12:49 pm

<ul>
{% for post in (site.tags["Easy"] | sort) %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>