---
template: default
---
<h2>Chronicling development of the <a href="https://github.com/bepisgang/zagnok">Zagnok project</a></h2>

The idea for Zagnok began as a hackathon project I worked on with my sister. We were big into Slackbots and big into being nerds, so we decided to try writing a bot that acted as a sort of DM for Slack-based [D&D](https://dnd.wizards.com)/[Pathfinder](https://paizo.com/pathfinder)-style encounters.

Our goal is to implement an API and accompanying robust data set that can be used to track encounter state or act as a searchable bestiary.

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
