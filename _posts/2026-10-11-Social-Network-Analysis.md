---
layout: posts
title: "Social Network Analysis Projectt"
date: 2026-10-11
mainColor: "#b7130b"
textColor: "#ff6232"
accentColor: "#560000"
bottone: "#b7130b"
fontTitoli: "Nosifer"
fontTesto: "Creepster"
image: /images/SocialNetwork.jpg
favicon: /images/favicons/halloween.png
titImage: /images/kghostface.gif
---
<style>
  :root { --paper: #630000; }
    /* Ghostface titolo */
  .hero h1 {
    background-position: center 20% !important;
  }
</style>

<div style="font-size:16px;">
   <h3>👻Co-occorrenza dei trope nei film Horror👻</h3>
   </div>

   <div class="center" style="margin-bottom:20px; margin-top:20px">
   <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to check it out! </a>
   </div>


<div style="width: min(1210px, 96vw); position: relative; left: 50%; transform: translateX(-50%);">

  <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(min(100%, 600px), 600px)); gap: 5px; justify-content: center; align-items: start;">
  <!-- Colonna sinistra -->
  <div>
    <!-- Pagina sinistra: Indice -->
    <div class="card" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
      <h2>Indice dei contenuti dell' elaborato</h2>
     <ul style="list-style-type: '💀 '; padding-left: 1.5rem;">
        <li>Introduzione</li>
        <li>Rete degli archetipi Horror
          <ul style="list-style-type: '🔪 '; padding-left: 1.5rem;">
            <li>Interpretazione del grafo di adiacenza
              <ul style="list-style-type: '😱 '; padding-left: 1.5rem;">
                <li>Cricche isolate</li>
                <li>Cluster centrale e Betweenness</li>
              </ul>
            </li>
            <li>Matrice di Modularità e Densità dei Cluster (Heatmap)
              <ul style="list-style-type: '🔪 '; padding-left: 1.5rem;">
                <li>Interpretazione dei risultati della matrice modulare
                  <ul style="list-style-type: '😱 '; padding-left: 1.5rem;">
                    <li>Cricche perfette</li>
                    <li>Cluster estesi e permeabili</li>
                  </ul>
                </li>
              </ul>
            </li>
          </ul>
        </li>
        <li>Riconoscere limiti e bias del lavoro
          <ul style="list-style-type: '🔪 '; padding-left: 1.5rem;">
            <li>Bias di selezione del dataset</li>
            <li>Resolution limit dell'algoritmo di Louvain</li>
          </ul>
        </li>
        <li>Conclusione</li>
      </ul>
    </div>
    <!-- Space tra i due riquadri -->
    <div style="height: 10px;"></div>
    <!-- Introduzione sotto l'Indice -->
    <div class="card" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
      <h2>Introduzione</h2>
        <p>
        In questo elaborato rispondo alle domande: "Quali cluster tematici esistono all'interno del cinema horror? E, soprattutto, esistono elementi narrativi ad esempio  trope come "possessione demoniaca" o "casa infestata" che fungono da ponte tra sotto-generi apparentemente distinti, collegando mondi narrativi diversi tra loro? " applicando tecniche viste a lezione ad un dataset di trope narrativi estratti dai principali film horror, costruendo una rete di co-occorrenza tra elementi tematici e applicando algoritmi di community detection e misure di centralità (in particolare la betweenness centrality) per identificare sia i cluster tematici sia gli archetipi "ponte" tra sottogeneri.
         </p>
    <h4 style="text-align: center;">...</h4>
      <div class="center">
        <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to continue </a>
      </div>
    </div>
    <!-- Space tra i due riquadri -->
    <div style="height: 10px;"></div>
    <!-- Ghostface-->
    <img src="{{ '/images/kghostface.gif' | relative_url }}" alt="ghostface" style="width: 100%; max-width: 400px; display: block; margin: 0 auto; border-radius: 25px;">
  </div>
  <!-- Pagina destra -->
  <div class="card" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
    <div class="indice" id="contenuto">Caricamento...
    </div>
  </div>
</div>

<script src="https://cdn.jsdelivr.net/npm/marked@12.0.2/marked.min.js"></script>
<script>
  (function () {
    const url = "https://raw.githubusercontent.com/AuroraCodingForFun/SocialNetworkAnalysisProject/refs/heads/master/README.md";
    const el = document.getElementById("contenuto");
    fetch(url)
      .then(r => {
        if (!r.ok) throw new Error(r.status);
        return r.text();
      })
      .then(md => {
        el.innerHTML = marked.parse(md);
      })
      .catch(err => { el.textContent = "Errore: " + err; });
  })();
</script>
