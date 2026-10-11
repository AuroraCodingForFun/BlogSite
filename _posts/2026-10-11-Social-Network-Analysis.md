---
layout: default
title: "My Social Network Analysis Project"
date: 2026-10-11
color1: "#b7130b"
color2: "#ff6232"
color3: "#560000"
image: /images/SocialNetwork.jpg
---
<div style="background-color: color1;>
   <div style="font-size:16px;">
   <h1>👻Co-occorrenza dei trope nei film Horror👻</h1>
   </div>

   <div class="center">
   <a class="button" href="https://github.com/AuroraCodingForFun/SocialNetworkAnalysisProject"> Click here to check it out! </a>
   </div>

   <div class="indice" style="background-color: white; padding: 16px 25px 25px 50px; border-radius: 25px;">
    <h2>Indice</h2>
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
          <li>Resolution limit dell’algoritmo di Louvain</li>
        </ul>
      </li> 
     <li>Conclusione </li>
    </ul>
  </div>

<br>
   <div>
   <h6>
    Immaginate di trovarvi in una fresca serata di inizio autunno, le foglie si ingialliscono, l’aria si raffredda e decidete di passare la serata guardando un film horror con i popcorn. Scorrendo  il catalogo della vostra piattaforma di intrattenimento preferita (o tra i DVD se siete all’antica) noterete la certa somiglianza tra le varie trame: Alcuni film parlano di case infestate, molti hanno come antagonisti gli Zombie, tanti parlano di serial killer che dà la caccia ad alcuni teenagers. Sorge spontanea una domanda: quali cluster tematici esistono all'interno del cinema horror? E, soprattutto, esistono elementi narrativi ad esempio  trope come "possessione demoniaca" o "casa infestata" che fungono da ponte tra sotto-generi apparentemente distinti, collegando mondi narrativi diversi tra loro? 
   </h6>
    <br>
   <h6>
   In questo elaborato rispondo a queste domande applicando tecniche viste a lezione ad un dataset di trope narrativi estratti dai principali film horror, costruendo una rete di co-occorrenza tra elementi tematici e applicando algoritmi di community detection e misure di centralità (in particolare la betweenness centrality) per identificare sia i cluster tematici sia gli archetipi "ponte" tra sottogeneri.
   </h6>
   </div>
</div>
