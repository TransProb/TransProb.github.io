---
layout: page
permalink: /publications/
title: publications
description:
nav: true
nav_order: 2
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
a {
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
  font-family: "Times New Roman", Times, serif !important;
  font-weight: 700 !important;
}

/* Justify paragraph text */
article p {
  text-align: justify;
  text-justify: inter-word;
  hyphens: auto;
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
    text-transform: uppercase;
  }
}
</style>
<p class="pub-note">
  <u>Underlined author</u> indicates myself; * indicates the corresponding author.
</p>
<div class="publications">

{% bibliography %}

</div>
