---
title: Accueil
layout: default
---

J'ai un nouveau blog sous Jekyll !

Liste des billets

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

Liste en Markdown

{% for post in site.posts %}
* [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
