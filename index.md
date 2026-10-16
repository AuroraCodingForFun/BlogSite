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
  top: 250px;
  right: 16px;
  box-sizing: border-box;
  width: 260px;
  max-height: calc(100vh - 120px);
  overflow-y: auto;
  padding: 16px 25px 30px 25px;
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
      <p>O</p>
    </aside>

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
  </div>
  {% endfor %}
</ul>
