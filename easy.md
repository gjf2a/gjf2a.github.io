---
layout: default
---

# Easy Assignments 12:31 pm

<ul>
{% for post in site.tags["Easy"] %}
{{ post }}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>