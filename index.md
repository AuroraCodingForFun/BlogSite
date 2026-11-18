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
<h1>Benvenuti nel mio blog </h1>
<h2> Ultimi post </h2>

<div id="myBtnContainer">
  <button class="btn active" onclick="filterSelection('all')"> Show all</button>
  <button class="btn" onclick="filterSelection('cars')"> Cars</button>
  <button class="btn" onclick="filterSelection('animals')"> Animals</button>
  <button class="btn" onclick="filterSelection('fruits')"> Fruits</button>
  <button class="btn" onclick="filterSelection('colors')"> Colors</button>
</div>

<ul class="post-list">
  {% for post in site.posts %}
  <li class="mbutton" style="background-color: {% if forloop.first %}#ffed3d{% else %}#edfcff{% endif %}; width: 100%; box-sizing: border-box;">
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
filterSelection("all")
function filterSelection(c) {
  var x, i;
  x = document.getElementsByClassName("filterDiv");
  if (c == "all") c = "";
  for (i = 0; i < x.length; i++) {
    w3RemoveClass(x[i], "show");
    if (x[i].className.indexOf(c) > -1) w3AddClass(x[i], "show");
  }
}

function w3AddClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    if (arr1.indexOf(arr2[i]) == -1) {element.className += " " + arr2[i];}
  }
}

function w3RemoveClass(element, name) {
  var i, arr1, arr2;
  arr1 = element.className.split(" ");
  arr2 = name.split(" ");
  for (i = 0; i < arr2.length; i++) {
    while (arr1.indexOf(arr2[i]) > -1) {
      arr1.splice(arr1.indexOf(arr2[i]), 1);     
    }
  }
  element.className = arr1.join(" ");
}

// Add active class to the current button (highlight it)
var btnContainer = document.getElementById("myBtnContainer");
var btns = btnContainer.getElementsByClassName("btn");
for (var i = 0; i < btns.length; i++) {
  btns[i].addEventListener("click", function(){
    var current = document.getElementsByClassName("active");
    current[0].className = current[0].className.replace(" active", "");
    this.className += " active";
  });
}
</script>
</body>
