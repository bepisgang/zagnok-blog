---
template: default
---
<h2>Chronicling development of the <a href="https://github.com/bepisgang/zagnok">Zagnok project</a></h2>

Zagnok began as a hackathon project for DMing Slack-based [D&D](https://dnd.wizards.com)/[Pathfinder](https://paizo.com/pathfinder)-style encounters.

Our goal is to implement a more general API and accompanying robust data set that can be used to track encounter state or act as a searchable bestiary.

This is a collection of thoughts as we travel this journey.

<h3>Recent Posts</h3>

<ul>
  <li>
  {% for post in site.posts %}
    <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
    <blockquote>{{ post.excerpt }}</blockquote>
    <br/>
  {% endfor %}
  </li>
</ul>
