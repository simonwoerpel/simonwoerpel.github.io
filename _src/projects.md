---
title: Projects
menu_title: projects
---

**`>>>>` [check out my publications on correctiv.org](https://correctiv.org/correctiv/redaktion/team/simon-woerpel/) `<<<<`**

we @ correctiv.org love to share our data & code with others. [this are some github-repos with data visualizations](https://github.com/correctiv?utf8=%E2%9C%93&q=viz&type=&language=)

{% if site.projects %}
{% assign projects = site.projects | sort: 'ordering' %}

## Here are a few in-depth descriptions about projects I worked on:

  <ul>
  {% for project in projects %}
    <li>
    <h3><a href="{{ project.url }}">{{ project.title }}</a></h3>
    <p>{{ project.teaser }}</p>
    <p>
    <a href="{{ project.url }}">> learn more</a>
      {% if project.external_url %} | visit: <a href="{{ project.external_url }}">{{ project.external_url }}</a>{% endif %}
    </p>
    </li>
  {% endfor %}
  </ul>
{% endif %}
