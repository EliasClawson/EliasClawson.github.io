---
layout: custom_home
title: "Elias Clawson"
permalink: /
heading_anchors: false
---




### Embedded Controls Engineer

Mission statement/Purpose here

Links to github and others

## Featured Projects

<div id="projectCarousel" class="carousel slide" data-ride="carousel" data-interval="5000">
  <div class="carousel-inner">
    {% assign featured_projects = site.projects | where: "featured", true %}
    {% for project in featured_projects %}
    <div class="carousel-item {% if forloop.first %}active{% endif %}">
      <a href="{{ project.url }}" style="text-decoration: none; color: inherit;">
        <div class="carousel-image" style="position:relative; height:400px; background:url('{{ project.image }}') center/cover;">
          <div class="carousel-caption" style="background: rgba(0,0,0,0.5); color: white; padding: 1rem; position: absolute; bottom: 0; width: 100%;">
            <h3>{{ project.title }}</h3>
            <p>{{ project.excerpt }}</p>
          </div>
        </div>
      </a>
    </div>
    {% endfor %}
  </div>

  <button class="carousel-control-prev custom-carousel-btn" type="button" data-target="#projectCarousel" data-slide="prev">
    <span class="carousel-control-prev-icon" aria-hidden="true"></span>
    <span class="sr-only">Previous</span>
  </button>
  <button class="carousel-control-next custom-carousel-btn" type="button" data-target="#projectCarousel" data-slide="next">
    <span class="carousel-control-next-icon" aria-hidden="true"></span>
    <span class="sr-only">Next</span>
  </button>
</div>

<style>
.custom-carousel-btn {
  width: 50px;
  height: 50px;
  background-color: rgba(0, 0, 0, 0.6);
  border: none;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  top: 50%;
  transform: translateY(-50%);
}

.carousel-control-prev {
  left: 20px;
}
.carousel-control-next {
  right: 20px;
}

.carousel-image {
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  overflow: hidden;
  background-size: cover;
}
</style>
