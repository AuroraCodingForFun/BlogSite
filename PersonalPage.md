---
layout: personal
title: "Super duper iper secret Personal page"
date: 2026-10-10
mainColor: "#ffffff"
textColor: "#111111"
accentColor: "#f9ed04"
fontTitoli: "Ballet"   
fontTitoliFile: "/images/fonts/Bartex.ttf"
fontTesto: "Italianno"
image: /images/sfondo.jpg
paper: "#ffcbb2"
pet: /images/nav/pets/ponyta.gif
---
<style>
  :root { --paper: #d6f2f5; }
  
.layout {
  display: block;
}
</style>
<nav>
  <a class="brand" href="https://github.com/AuroraCodingForFun">
    <img src="{{ '/images/nav/Github.gif' | relative_url }}" width="55" height="55" alt="Github">
  </a>
  <h6>Github</h6>
  <a href="{{ '/' | relative_url }}">
      <img src="{{ '/images/nav/Casa.gif' | relative_url }}" width="55" height="55" alt="Home">
  </a>
  <h6>Home</h6>
  <button onclick="boringMode()" style="background: none; border: none; padding: 0; margin: 0;">
     <img src="{{ '/images/nav/BoringMode.gif' | relative_url }}" width="55" height="55" alt="dark mode">
  </button>
  <h6>Dark mode</h6>
</nav>
