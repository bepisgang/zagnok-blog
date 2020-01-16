---
template: default
---

<h3>Recent Posts</h3>

<ul>
  <li>
  {% for post in site.posts %}
    <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
      {{ post.excerpt }}
  {% endfor %}
  </li>
</ul>
