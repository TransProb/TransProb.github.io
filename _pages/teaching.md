---
layout: page
permalink: /teaching/
title: teaching
description: Course materials, schedules, and resources for classes taught.
nav: true
nav_order: 6
calendar: true
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
This page displays a collection of courses with detailed schedules, materials, and resources. You can organize your courses by years, terms, or topics.

{% include calendar.liquid calendar_id='test@gmail.com' timezone='Asia/Shanghai' %}

{% include courses.liquid %}
