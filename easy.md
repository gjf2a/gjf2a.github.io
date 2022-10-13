---
layout: default
---

# Easy Assignments 12:15 pm

{{site.tags["Easy"]}}

<ul>
{% for post in {{site.tags | find: "Easy"}}[1] %}
<li><a href="{{ post.url }}">{{ post.title }}</a></li>
{% endfor %}
</ul>