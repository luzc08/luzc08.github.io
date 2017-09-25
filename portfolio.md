---
title: portfolio
permalink: /portfolio/
---

{% for project in site.projects %}
<div class="project ">
    <div class="thumbnail">
        <a href="{{ site.baseurl }}{{ project.url }}">
        {% if project.image %}
        <img class="thumbnail" src="{{ site.baseurl }}{{ project.image }}"/>
        {% else %}
        <div class="thumbnail blankbox"></div>
        {% endif %}
        <span>
            <h1>{{ project.title }}</h1>
            <br/>
            <p>{{ project.description }}</p>
        </span>
        </a>
    </div>
</div>

{% endfor %}
