---
layout: page
permalink: /updates/
title: updates
description:
nav: false
---

<style>
/* Times New Roman */
body,
p,
h1,
h2,
h3,
h4,
h5,
h6,
li,
a,
strong,
b,
span {
  font-family: "Times New Roman", Times, serif !important;
}

/* Normal body text */
body,
p,
li {
  font-weight: 400;
}

/* Bold text */
strong,
b {
  font-weight: 700 !important;
}

/* Hide page title and description */
.post-header,
.post-title,
.post-description {
  display: none !important;
}

/* Center navigation menu */
@media (min-width: 992px) {
  .navbar {
    padding-top: 30px !important;
    padding-bottom: 30px !important;
  }

  .navbar-nav {
    position: absolute;
    left: 50%;
    transform: translateX(-50%);
    margin: 0 !important;
  }

  .navbar-nav .nav-link {
    font-family: "Times New Roman", Times, serif !important;
    text-transform: uppercase;
  }
}
</style>

<div class="news">
  {% include news.liquid %}
</div>
