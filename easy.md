---
layout: default
---

# Easy Assignments 12:53 pm

<ul>
{% for post in site.tags["Easy"] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>