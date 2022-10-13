---
layout: default
---

# Easy Assignments 12:23 pm

<ul>
{% for post in site.tags["Easy"][1] %}
{{ post }}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>