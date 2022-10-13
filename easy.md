---
layout: default
---

# Easy Assignments 12:20 pm

<ul>
{% for post in site.tags["Easy"][1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>