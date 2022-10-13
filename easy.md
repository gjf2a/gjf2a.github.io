---
layout: default
---

# Easy Assignments

<ul>
{% for post in {{site.tags | find: "Easy"}}[1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>