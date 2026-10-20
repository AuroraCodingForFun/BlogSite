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
  
.layout {
  display: block;
}
</style>

<div>
<h1>Benvenuti nel mio blog </h1>
<h2> Ultimi post </h2>
<ul class="post-list">
  {% for post in site.posts %}
  <a href="{{ post.url | relative_url }}" style="text-decoration: none; display: block; width: 100%; box-sizing: border-box;">
    <li class="button" style="background-color: {% if forloop.first %}#5deff4{% else %}#edfcff{% endif %}; width: 100%; box-sizing: border-box;">
      <div style="display: flex; align-items: center; justify-content: space-between;">
        <span>
          <b style="color: #3a6b35; font-size: 2rem;">{{ post.title }}</b>
          <small style="color: #3a6b35">({{ post.date | date: "%d/%m/%Y" }})</small>
        </span>
        <img src="{{ '/images/rocket.gif' | relative_url }}" width="75" height="75" alt="rocket" style="border-radius: 50%;">
      </div>
    </li>
  </a>
{% endfor %}
</ul>
</div>
