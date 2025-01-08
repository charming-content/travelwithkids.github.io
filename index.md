---
layout: default
title: "home"
---

# Hello and Welcome to our "Traveling the World with Kids" Travel Blog!

<div class="image-container">
  <img src="{{ 'assets/images/beautiful-taiwan-popumon-hehuanshan-east-peak.jpg' | relative_url }}" alt="Picture">
</div>

Hi, We are the CharMing family, and this is our travel blog where we share my experiences from exploring the world with our kids. From the bustling streets of Taipei to the serene beaches of Malaysia, We will take you on a journey to discover new food places, cultures, and adventures. Tips and lesson learnt so that you will not repeat our mistakes :)

## CharMing's Travelling Logs and Itineraries :)
{% for post in site.posts %}
  * [{{ post.title }}]({{ post.url }}) - {{ post.date | date: "%B %d, %Y" }}
{% endfor %}


<h2>Cooking Recipes</h2>
<ul>
  {% for post in site.categories.recipes %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
