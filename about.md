---
template: default
---

### Recent Posts

<ul>
  <li>
  {% for post in site.posts %}
  <h4>{% post.title %}</h4>
      {% post.excerpt %}
  {% endfor %}
  </li>
</ul>
