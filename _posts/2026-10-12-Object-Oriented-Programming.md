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

<style> :root { --paper: #100b08; } </style>

<div>
   <div style="font-size:16px;">
   <h1>Objected Oriented Programming Exham</h1>
   </div>

   <div class="center">
   <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to check it out! </a>
   </div>

   <div class="indice" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
      
<div id="contenuto">Caricamento...</div>

<script src="https://cdn.jsdelivr.net/npm/marked@12.0.2/marked.min.js"></script>
<script>
  const url = "https://raw.githubusercontent.com/AuroraCodingForFun/OOP-Exercises/refs/heads/main/README.md";

  fetch(url)
    .then(r => r.text())
    .then(md => {
      document.getElementById("contenuto").innerHTML = marked.parse(md);
    })
    .catch(err => {
      document.getElementById("contenuto").textContent = "Errore: " + err;
    });
</script>
  </div>

<br>

  <aside style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
    <h2>Side content</h2>
   <p>
  This should be on the side of the page, why are you not? How many goats do I have to sacrifice?
   </p>
    <h4 style="text-align: center;">...</h4>
       <div class="center">
       <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to continue </a>
       </div>
   </aside>
</div>
