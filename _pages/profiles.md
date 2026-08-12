---
layout: profiles
permalink: /people/
title: people
description: members of the lab or group
nav: true
nav_order: 7
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
profiles:
  # if you want to include more than one profile, just replicate the following block
  # and create one content file for each profile inside _pages/
  - align: right
    image: prof_pic.jpg
    content: about_einstein.md
    image_circular: false # crops the image to make it circular
    more_info: >
      <p>555 your office number</p>
      <p>123 your address street</p>
      <p>Your City, State 12345</p>
  - align: left
    image: prof_pic.jpg
    content: about_einstein.md
    image_circular: false # crops the image to make it circular
    more_info: >
      <p>555 your office number</p>
      <p>123 your address street</p>
      <p>Your City, State 12345</p>
---
