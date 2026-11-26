---
title: Benvenuti!
layout: default
image: /images/copertina.jpg
color1: "#001044"
color2: "#C8C367"
color3: "#615F31"
---
<style>
 :root { --paper: url('{{ 'images/matrix-code.gif' | relative_url }}') center / cover no-repeat; }
  
.layout {
  display: block;
}
</style>
<body>
<h1> 🌟 Benvenuti nel mio blog 🌟 </h1>
<h2> Ultimi post: </h2>

<div class="dropdown">
  <button onclick="FunzioneDropdown()" class="dropbtn">Filtra per linguaggio di programmazione:</button>
  <div id="myDropdown" class="dropdown-content">
     <div class="btnContainer" id="BtnContainer">
       <button class="btnall" data-filter="all">Tutti</button>
       {% for tag in site.tags %}
       {% assign name = tag[0] %}
       {% assign info = site.data.tags[name] %}
       <button class="btn" data-filter="{{ name | slugify }}" aria-label="{{ name }}" title="{{ name }}">
         {% if info.logo %}<img src="{{ info.logo | relative_url }}" alt="{{ name }}" class="tag-logo" style="height: auto; width: 50px"> <p> {{ name }} </p>{% endif %}
       </button>
     {% endfor %}
     </div>
  </div>
</div>
    
<ul class="post-list">
  {% for post in site.posts %}
  <li class="mbutton" data-tags="{% for t in post.tags %}{{ t | slugify }} {% endfor %}" style="background-color: {% if forloop.first %}#ffed3d{% else %}#edfcff{% endif %}; width: 100%; box-sizing: border-box;">
    {% if forloop.first %}
      <span class="ribbon">NEW</span>
    {% endif %}
    <a href="{{ post.url | relative_url }}" style="text-decoration: none; display: block; width: 100%; box-sizing: border-box;">
      <div style="display: flex; align-items: center; justify-content: start; gap: 10px">
        <img src="{{post.image | relative_url}}" alt="thumbnail">
        <span>
          <b style="color: #3a6b35; font-size: 1.7rem;">{{ post.title }}</b>
          <small style="color: #3a6b35">{{ post.desc}}</small>
        </span>
      </div>
    </a>
  </li>
  {% endfor %}
</ul>

<script>
document.querySelectorAll('#BtnContainer .btn').forEach(function (btn) {
  btn.addEventListener('click', function () {
    var current = document.querySelector('#BtnContainer .active');
    if (current) current.classList.remove('active');
    btn.classList.add('active');

    var f = btn.dataset.filter;
    document.querySelectorAll('.post-list li').forEach(function (li) {
      var tags = li.dataset.tags.trim().split(' ');
      li.style.display = (f === 'all' || tags.includes(f)) ? '' : 'none';
    });
  });
});

 /* When the user clicks on the button, 
toggle between hiding and showing the dropdown content */
function FunzioneDropdown() {
  document.getElementById("myDropdown").classList.toggle("show");
}

// Close the dropdown if the user clicks outside of it
window.onclick = function(event) {
  if (!event.target.matches('.dropbtn')) {
    var dropdowns = document.getElementsByClassName("dropdown-content");
    var i;
    for (i = 0; i < dropdowns.length; i++) {
      var openDropdown = dropdowns[i];
      if (openDropdown.classList.contains('show')) {
        openDropdown.classList.remove('show');
      }
    }
  }
}
</script>
</body>
