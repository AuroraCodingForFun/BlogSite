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
  
.indice {
  flex: 1;
  min-width: 0;
  background-color: white;
  padding: 16px 25px 30px 25px;
  border-radius: 25px;
}

aside.laterale {
  position: fixed;
  top: 10px;
  right: 16px;
  box-sizing: border-box;
  width: 260px;
  max-height: calc(100vh - 120px);
  overflow-y: auto;
  padding: 10px 10px 10px 10px;
  background-color: white;
  border-radius: 25px;
  font-style: italic;
  z-index: 10;
}

  @media (max-width: 1100px) {
  aside.laterale {
    position: static;
    width: auto;
    max-height: none;
    margin-top: 24px;
  }
}
</style>

<div>
    <aside class="laterale">
      <img src="{{ '/images/copertina.jpg' | relative_url }}" alt="Copertina del blog">
    </aside>
<h1>Benvenuti nel mio blog </h1>
<h2> Ultimi post </h2>
<ul class="post-list">
  {% for post in site.posts %}
  <li style="background-color: {% if forloop.first %}#5deff4{% else %}#edfcff{% endif %}">
    <div class="button" style="display: flex; align-items: center; justify-content: space-between;">
      <span>
        <a href="{{ post.url | relative_url }}"><b style="color: #3a6b35">{{ post.title }}</b></a>
        <small style="color: #3a6b35">({{ post.date | date: "%d/%m/%Y" }})</small>
      </span>
      <img src="{{ '/images/rocket.gif' | relative_url }}" width="75" height="75" alt="rocket" style="border-radius: 50%;">
    </div>
  </li>
{% endfor %}
</ul>
</div>
