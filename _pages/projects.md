---
layout: page
title: projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: False
nav_order: 3
display_categories: [work, fun]
horizontal: false
---
<style>
body,
p,
h1,
h2,
h3,
h4,
h5,
h6,
li,
a {
  font-family: "Times New Roman", Times, serif !important;
}

/* 普通正文 */
body,
p,
li {
  font-weight: 400;
}

/* 只有 Markdown 的 **文字** 加粗 */
strong,
b {
  font-family: "Times New Roman", Times, serif !important;
  font-weight: 700 !important;
}
  
article p {
  text-align: justify;
  text-justify: inter-word;
  hyphens: auto;
}

.profile .more-info,
.profile .more-info p {
  font-family: "Times New Roman", Times, serif !important;
  text-align: left;
}

/* Center the navigation menu */
@media (min-width: 992px) {
  .navbar {
    padding-top: 30px !important;
    padding-bottom: 30px !important;
  }
}

  .navbar-nav {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    margin: 0 !important;
  }

  .navbar-nav .nav-link {
    text-transform: uppercase;
  }
}
</style>



<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_projects = site.projects | where: "category", category %}
  {% assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->

{% assign sorted_projects = site.projects | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>
