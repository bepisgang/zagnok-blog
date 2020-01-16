---
template: default
---
<h1>Chronicling development of the <a href="https://github.com/bepisgang/zagnok">Zagnok project</a></h1>

<h2>Recent Posts</h2>

<ul>
  <li>
  {% for post in site.posts %}
    <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
    <blockquote>{{ post.excerpt }}</blockquote>
    <br/>
  {% endfor %}
  </li>
</ul>
