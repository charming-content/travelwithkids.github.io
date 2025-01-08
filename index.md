---
layout: default
title: "Home"
---
<h1>{{ site.title }}</h1>

<div class="container">
  <div class="travel-posts">
    <h2>Travel Posts</h2>
    <ul>
      {% for post in site.categories.travel %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
        </li>
      {% endfor %}
    </ul>
  </div>

  <div class="recipes-posts">
    <h2>Cooking Recipes</h2>
    <ul>
      {% for post in site.categories.recipes %}
        <li>
          <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
