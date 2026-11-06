---
layout: personal
title: "First Post"
date: 2026-10-10
mainColor: "#ffb3c0"
textColor: "#f94563"
accentColor: "#ae0068"
fontTitoli: "Ballet"   
fontTitoliFile: "/images/fonts/Bartex.ttf"
fontTesto: "Italianno"
image: /images/header/scary.jpg
paper: "#ffcbb2"
pet: /images/nav/pets/ponyta.gif
---
<style>
  :root { --paper: #14281d; }
  
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

<h2>Contact me</h2>

<div style="background-color: white">
<form
  action="https://formspree.io/f/mgaaqgzz"
  method="POST"
>
  <label>
    Your email:
    <input type="email" name="email">
  </label>
  <label>
    Your message:
    <textarea name="message"></textarea>
  </label>
  <!-- your other form fields go here -->
  <button type="submit">Send</button>
</form>
</div>
