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
  top: 0;
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
  <div style="font-size:16px;">
    <h1>Objected Oriented Programming Exham</h1>
  </div>
  <div class="center">
    <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject">Click here to check it out!</a>
  </div>

  <div class="layout">
    <div class="indice">
      <div id="contenuto">Caricamento...</div>
    </div>
    <aside class="laterale">
      <h2>Side content</h2>
      <p>Ciaooo</p>
      <h4 style="text-align: center;">...</h4>
      <div class="center">
        <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject">Click here to continue</a>
      </div>
    </aside>

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
