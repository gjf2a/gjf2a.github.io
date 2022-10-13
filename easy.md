---
layout: default
---

# Easy Assignments 12:13 pm

{{site.tags | find: "Easy"}}

<ul>
{% for post in {{site.tags | find: "Easy"}}[1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>