---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults


layout: splash
title: "Welcome to My Site"
permalink: /
---



This is where I'll show off some projects and maybe have useful links like my github.

## Featured Projects

<div id="projectCarousel" class="carousel slide" data-ride="carousel">
  <div class="carousel-inner">
    {% assign featured_projects = site.projects | where: "featured", true %}
    {% for project in featured_projects %}
    <div class="carousel-item {% if forloop.first %}active{% endif %}">
      <a href="{{ project.url }}">
        <h3>{{ project.title }}</h3>
        <p>{{ project.excerpt }}</p>
      </a>
    </div>
    {% endfor %}
  </div>
  <a class="carousel-control-prev" href="#projectCarousel" role="button" data-slide="prev">‹</a>
  <a class="carousel-control-next" href="#projectCarousel" role="button" data-slide="next">›</a>
</div>
