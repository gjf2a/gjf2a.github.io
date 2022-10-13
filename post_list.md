---
layout: default
---

<!-- Credit: https://learn.cloudcannon.com/jekyll/list-posts/ -->

# Posts

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
      <!-- - <time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time> -->
    </li>
  {% endfor %}
</ul>

# Tags

{% for tag in site.tags %}
## {{ tag | first }}
<!-- Bad idea {{ tag | last }} -->
  <ul>
  {% for post in {{ tag | last }} %}
  <li> {{ post }}
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

