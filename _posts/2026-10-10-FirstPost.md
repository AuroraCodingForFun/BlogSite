---
layout: posts
title: "First Post"
date: 2026-10-10
color1: "#ffb3c0"
color2: "#f94563"
color3: "#f945bd"
image: /images/Barbie.jpg
paper: "#ffcbb2"
---
<style>
     
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
      <h2> "More content:"</h2>
     {% for post in site.posts %}
         <a href="{{ post.url | relative_url }}" style="text-decoration: none; display: block;">
          <li class="button" style="background-color: {% if forloop.first %}#5deff4{% else %}#edfcff{% endif %}">
           <div style="display: flex; align-items: center; justify-content: space-between;">
             <span>
               <b style="color: #3a6b35">{{ post.title }}</b>
               <small style="color: #3a6b35">({{ post.date | date: "%d/%m/%Y" }})</small>
             </span>
           </div>
         </li>
       </a>
     {% endfor %}
</aside>
<h1>Ciao? Quindi è così che si fa un post!</h1>
   <div class="indice" style="background-color: white; padding: 16px 25px 30px 50px; border-radius: 25px;">
<p>Oggi ho finalmente deciso di iniziare a fare questo piccolo blog, forse sono 10 anni in ritardo rispetto a quando i blog andavano di moda ma non importa. Sicuramente mi stancherò di questa cosa o mi dimenticherò a breve.</p>
<br>
<p> Mi piace molto comunque provare a vedere e registrare da qualche parte i miei progressi nel mondo dell'informatica quindi userò di sicuro questa piattaforma.</p>
<br>
<h6>Non aspettarti molto da questo progetto</h6>
   </div>
</div>
