---
layout: default
---

<!-- Credit: https://learn.cloudcannon.com/jekyll/list-posts/ -->

# Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <!-- - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> -->
    </li>
  {% endfor %}
</ul>

# Tags 9:20 AM

{% for tag in site.tags %}
## {{ tag[0] }}
  <ul>
  {% for post in tag[1] %}
  <li> <a href="{{ post.url }}"> {{ post.title }} </a>
  {% endfor %}
  </ul>
{% endfor %}

# Site
{{ site.tags }}

# Page
{{ page.tags }}

# Loop
{% for tag in site.tags %}
  Name: {{ tag | first }},
  count: {{ tag | last | size}}
{% endfor %}

