---
layout: posts
title: "My Social Network Analysis Project"
date: 2026-10-11
color1: "#b7130b"
color2: "#ff6232"
color3: "#560000"
button: "#b7130b"
image: /images/SocialNetwork.jpg
favicon: /images/favicons/halloween.png
---
<style>
  :root { --paper: #630000; }
</style>

<div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(16rem, 1fr)); gap: 0;">

<div style="font-size:16px;">
   <h1>👻Co-occorrenza dei trope nei film Horror👻</h1>
   </div>

   <div class="center">
   <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to check it out! </a>
   </div>

  <!-- Pagina sinistra -->
  <div style="background-color: white; color: #2b0a0a; padding: 1.5rem; border-radius: 25px 0 0 25px;">
    <h2>Indice dei contenuti</h2>
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
        </ul>
      </li>
    </ul>
  </div>

  <!-- Pagina destra -->
  <div style="background-color: white; color: #2b0a0a; padding: 1.5rem; border-radius: 0 25px 25px 0; box-shadow: inset 12px 0 12px -12px rgba(0,0,0,0.35);">
    <h2>Seconda parte</h2>
    <ul style="list-style-type: '💀 '; padding-left: 1.5rem;">
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
      <li>Riconoscere limiti e bias del lavoro
        <ul style="list-style-type: '🔪 '; padding-left: 1.5rem;">
          <li>Bias di selezione del dataset</li>
          <li>Resolution limit dell'algoritmo di Louvain</li>
        </ul>
      </li>
      <li>Conclusione</li>
    </ul>
  </div>

</div>
  <div style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
    <h2>Introduzione</h2>
   <p>
  In questo elaborato rispondo alle domande: "Quali cluster tematici esistono all'interno del cinema horror? E, soprattutto, esistono elementi narrativi ad esempio  trope come "possessione demoniaca" o "casa infestata" che fungono da ponte tra sotto-generi apparentemente distinti, collegando mondi narrativi diversi tra loro? " applicando tecniche viste a lezione ad un dataset di trope narrativi estratti dai principali film horror, costruendo una rete di co-occorrenza tra elementi tematici e applicando algoritmi di community detection e misure di centralità (in particolare la betweenness centrality) per identificare sia i cluster tematici sia gli archetipi "ponte" tra sottogeneri.
   </p>
    <h4 style="text-align: center;">...</h4>
       <div class="center">
       <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to continue </a>
       </div>
   </div>
</div>
