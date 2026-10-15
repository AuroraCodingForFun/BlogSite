---
title: Benvenuti!
layout: default
image: /images/copertina.jpg
color1: "#001044"
color2: "#C8C367"
color3: "#615F31"
---
<style>
  :root { --paper: #14281d; }
</style>

Benvenuti nel mio blog

## Ultimi post

<ul class="post-list">
  
  {% for post in site.posts %}
    <li style=" background-color: lightblue">
      <div>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <small>({{ post.date | date: "%d/%m/%Y" }})</small>
      </div>
    </li>
  
  {% endfor %}
</ul>
