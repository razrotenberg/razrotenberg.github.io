---
layout: page
title: Projects
permalink: /projects/
---
<style type="text/css">
  .container {
    display: flex;
  }

  /* small screens */
  @media screen and (max-width: 500px) {
    .on-small-screen {
      display: grid;
    }
    a.logo {
      text-align: center;
    }
    img.logo {
      margin-top: 20px;
      margin-bottom: 50px;
      width: 70%;
      align: center;
    }
    .col.right {
      display: none;
    }
  }

  /*  big screens */
  @media screen and (min-width: 500px) {
    .on-small-screen {
      display: none;
    }
    img.logo {
      width: 80%;
    }
    .col {
      flex: 1;
    }
    .col.right {
      text-align: right;
      align-self: center;
    }
  }
</style>

{% for project in site.projects %}

<hr>

<div class="container">
  <div class="col left">
    <h3 class="project-name">{{project.title}}</h3>
    <h5>{{project.time}}</h5>
    <div class="on-small-screen">
      <a href="{{project.permalink}}" class="logo">
        <img class="logo" src="/assets/logos/{{project.logo}}">
      </a>
    </div>
    <p>{{project.description}}.</p>
    <a href="{{project.permalink}}" class="button">Read more...</a>
  </div>
  <div class="col right">
    <a href="{{project.permalink}}">
      <img class="logo" src="/assets/logos/{{project.logo}}">
    </a>
  </div>
</div>

{% endfor %}
