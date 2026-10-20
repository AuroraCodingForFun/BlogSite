---
layout: posts
title: "Studying Java (Object Oriented Exham)"
date: 2026-10-11
color1: "#100b08"
color2: "#dd985f"
color3: "#855d3a"
image: /images/Java.jpg
favicon: /images/favicons/java-logo.png
---
<style>
:root { --paper: #100b08; }
</style>

<div>
  <div style="font-size:16px;">
    <h1>Objected Oriented Programming Exham</h1>
  </div>
  <div class="center">
    <a class="button" href=https://github.com/AuroraCodingForFun/OOP-Exercises">Click here to check it out!</a>
  </div>
  <br>
  <div class="layout" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
    <div class="indice">
      <div id="contenuto">Caricamento...</div>
    </div>
  </div>
  <br>
</div>

<script src="https://cdn.jsdelivr.net/npm/marked@12.0.2/marked.min.js"></script>
<script>
  (function () {
    const url = "https://raw.githubusercontent.com/AuroraCodingForFun/OOP-Exercises/refs/heads/main/README.md";
    const el = document.getElementById("contenuto");
    fetch(url)
      .then(r => {
        if (!r.ok) throw new Error(r.status);
        return r.text();
      })
      .then(md => { el.innerHTML = marked.parse(md); })
      .catch(err => { el.textContent = "Errore: " + err; });
  })();
</script>
