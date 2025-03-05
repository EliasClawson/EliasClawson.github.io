---
layout: custom_home
title: "Elias Clawson"
permalink: /
heading_anchors: false
---




### Embedded and Controls Engineer
Bachelor of Science in Electrical and Computer Engineering (BS ECE - BYU)

Mission statement/Purpose here. Something else?

<a href="https://github.com/eliasclawson" target="_blank" aria-label="GitHub">
    <svg height="48" width="48" fill="currentColor" aria-hidden="true" viewBox="0 0 16 16">
        <path d="M8 0C3.58 0 0 3.58 0 8a8 8 0 005.47 7.59c.4.07.55-.17.55-.38v-1.33C4.07 14.41 3.6 13.13 3.6 13.13c-.36-.91-.88-1.15-.88-1.15-.72-.49.06-.48.06-.48.8.06 1.22.82 1.22.82.7 1.2 1.84.85 2.29.65.07-.51.27-.85.49-1.05-1.75-.2-3.58-.88-3.58-3.93 0-.87.31-1.58.82-2.14-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82a7.7 7.7 0 014 0c1.53-1.03 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.14 0 3.06-1.84 3.73-3.6 3.93.28.24.53.72.53 1.45v2.15c0 .21.15.46.55.38A8 8 0 0016 8c0-4.42-3.58-8-8-8z"/>
    </svg>
</a>
<a href="https://www.linkedin.com/in/elias-clawson" target="_blank" aria-label="LinkedIn" style="margin-left: 12px;">
    <svg height="48" width="48" fill="currentColor" aria-hidden="true" viewBox="0 0 16 16">
        <path d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zM4.943 13.2V6.169H2.542V13.2h2.401zM3.743 5.193c.837 0 1.357-.554 1.357-1.248-.015-.708-.52-1.249-1.34-1.249-.82 0-1.357.541-1.357 1.249 0 .694.52 1.248 1.31 1.248h.03zm4.09 8.007V9.359c0-.206.015-.413.075-.56.164-.413.54-.84 1.17-.84.825 0 1.155.633 1.155 1.56v3.681h2.401V9.26c0-2.099-1.11-3.074-2.589-3.074-1.207 0-1.735.826-2.034 1.401h.015V6.17H5.844c.03.634 0 7.03 0 7.03h2.402z"/>
    </svg>
</a>


## Featured Projects

<div id="projectCarousel" class="carousel slide" data-ride="carousel" data-interval="5000">
  <div class="carousel-inner">
    {% assign featured_projects = site.projects | where: "featured", true %}
    {% for project in featured_projects %}
    <div class="carousel-item {% if forloop.first %}active{% endif %}">
      <a href="{{ project.url }}" style="text-decoration: none; color: inherit;">
        <div class="carousel-image" style="position:relative;   background:url('{{ project.image }}') center/cover;">
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
  height: auto;
  max-width: 100%;
  object-fit: cover;
}

.carousel-caption {
  transition: opacity 0.5s ease-in-out;
}

.carousel-item {
  transition: transform 0.5s ease-in-out;
}

</style>


## What I Do

- **Embedded Systems Development:** Designing and programming microcontroller-based solutions.
- **Control Systems Engineering:** Building autonomous systems for various applications.