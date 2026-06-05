<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Energia Eólica na Zona Rural</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

:root{
--gold:#FFD700;
--gold2:#ffb300;
--dark:#050505;
--dark2:#121212;
--white:#ffffff;
}

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:"Segoe UI",sans-serif;
}

html{
scroll-behavior:smooth;
}

body{

background:
linear-gradient(
-45deg,
#000000,
#111111,
#1a1a1a,
#3d3000
);

background-size:400% 400%;
animation:gradient 15s ease infinite;

color:white;
overflow-x:hidden;
}

@keyframes gradient{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

/* MENU */

nav{
position:fixed;
top:0;
width:100%;
padding:20px 8%;
display:flex;
justify-content:space-between;
align-items:center;
z-index:1000;

backdrop-filter:blur(12px);
background:rgba(0,0,0,.35);
}

.logo{
font-size:1.4rem;
font-weight:bold;
color:var(--gold);
}

nav ul{
display:flex;
gap:30px;
list-style:none;
}

nav a{
color:white;
text-decoration:none;
transition:.3s;
}

nav a:hover{
color:var(--gold);
}

/* HERO */

.hero{

height:100vh;

background:
linear-gradient(rgba(0,0,0,.65),rgba(0,0,0,.75)),
url("https://images.unsplash.com/photo-1466611653911-95081537e5b7?auto=format&fit=crop&w=2000&q=80");

background-size:cover;
background-position:center;
background-attachment:fixed;

display:flex;
justify-content:center;
align-items:center;

padding:40px;
}

.hero-card{

max-width:1000px;

text-align:center;

padding:60px;

background:rgba(255,255,255,.08);

backdrop-filter:blur(15px);

border:1px solid rgba(255,255,255,.1);

border-radius:25px;

box-shadow:
0 0 20px rgba(255,215,0,.25),
0 0 50px rgba(255,215,0,.15);
}

.hero h1{

font-size:4rem;
color:var(--gold);
margin-bottom:20px;
}

.hero p{

font-size:1.3rem;
line-height:1.8;
max-width:800px;
margin:auto;
}

.btn{

display:inline-block;
margin-top:35px;

padding:15px 35px;

background:var(--gold);
color:black;

font-weight:bold;
text-decoration:none;

border-radius:40px;

transition:.3s;
}

.btn:hover{

transform:translateY(-5px);

box-shadow:
0 0 20px var(--gold),
0 0 40px rgba(255,215,0,.5);
}

/* INDICADORES */

.stats{

display:grid;

grid-template-columns:
repeat(auto-fit,minmax(220px,1fr));

gap:25px;

padding:80px 10%;
}

.stat{

text-align:center;

padding:30px;

background:rgba(255,255,255,.05);

border-radius:20px;

transition:.4s;
}

.stat:hover{

transform:translateY(-8px);

box-shadow:
0 0 20px rgba(255,215,0,.3);
}

.number{

font-size:3rem;
font-weight:bold;
color:var(--gold);
}

.label{
margin-top:10px;
}

/* SEÇÕES */

section{

padding:100px 10%;
}

.section-title{

font-size:2.5rem;
color:var(--gold);

margin-bottom:30px;
}

.text{

font-size:1.15rem;
line-height:2;
}

/* BENEFÍCIOS */

.benefits{

display:grid;
grid-template-columns:
repeat(auto-fit,minmax(250px,1fr));

gap:30px;
margin-top:40px;
}

.card{

padding:30px;

background:rgba(255,255,255,.05);

border-radius:20px;

transition:.4s;
}

.card:hover{

transform:translateY(-10px);

box-shadow:
0 0 20px rgba(255,215,0,.25);
}

.card h3{

color:var(--gold);
margin:15px 0;
}

/* PERSONAGENS */

.people{

display:flex;
flex-wrap:wrap;
justify-content:center;
gap:40px;
margin-top:50px;
}

.person{

text-align:center;
max-width:250px;
}

.avatar{

font-size:80px;
animation:float 4s ease-in-out infinite;
}

@keyframes float{

0%{transform:translateY(0);}
50%{transform:translateY(-12px);}
100%{transform:translateY(0);}
}

/* TABELA */

table{

width:100%;
margin-top:30px;

border-collapse:collapse;
}

th{

background:var(--gold);
color:black;
padding:15px;
}

td{

padding:15px;
border-bottom:
1px solid rgba(255,255,255,.1);
}

/* GRAFICO */

.chart-container{

background:white;
padding:30px;
border-radius:25px;
}

/* FOOTER */

footer{

padding:50px;
text-align:center;

background:black;
}

footer h3{
color:var(--gold);
margin-bottom:10px;
}

/* REVEAL */

.reveal{

opacity:0;
transform:translateY(60px);

transition:all .8s ease;
}

.reveal.active{

opacity:1;
transform:translateY(0);
}

@media(max-width:768px){

.hero h1{
font-size:2.5rem;
}

.hero-card{
padding:35px;
}

nav ul{
display:none;
}

}

</style>
</head>
<body>

<nav>

<div class="logo">
🌬️ Energia Eólica
</div>

<ul>
<li><a href="#intro">Introdução</a></li>
<li><a href="#beneficios">Benefícios</a></li>
<li><a href="#planejamento">5W2H</a></li>
<li><a href="#grafico">Gráfico</a></li>
</ul>

</nav>

<header class="hero">

<div class="hero-card">

<h1>Energia Eólica na Zona Rural</h1>

<p>
Uma solução sustentável para reduzir custos,
aumentar a autonomia energética das propriedades
rurais e promover o desenvolvimento ambiental.
</p>

<a href="#intro" class="btn">
Explorar Projeto
</a>

</div>

</header>

<section class="stats">

<div class="stat">
<div class="number" data-target="90">0</div>
<div class="label">Economia Financeira</div>
</div>

<div class="stat">
<div class="number" data-target="95">0</div>
<div class="label">Sustentabilidade</div>
</div>

<div class="stat">
<div class="number" data-target="85">0</div>
<div class="label">Autonomia Energética</div>
</div>

<div class="stat">
<div class="number" data-target="70">0</div>
<div class="label">Geração de Empregos</div>
</div>

</section>

<section id="intro" class="reveal">

<h2 class="section-title">Introdução</h2>

<p class="text">

A energia eólica utiliza a força dos ventos para
produzir eletricidade por meio de aerogeradores.

Sua implementação na zona rural permite reduzir
custos operacionais, fortalecer a independência
energética e contribuir para a preservação ambiental.

</p>

</section>

<section id="beneficios" class="reveal">

<h2 class="section-title">Benefícios</h2>

<div class="benefits">

<div class="card">
<h3>💰 Economia</h3>
<p>Redução significativa das despesas energéticas.</p>
</div>

<div class="card">
<h3>🌱 Sustentabilidade</h3>
<p>Fonte limpa e renovável.</p>
</div>

<div class="card">
<h3>⚡ Autonomia</h3>
<p>Menor dependência da rede elétrica.</p>
</div>

<div class="card">
<h3>👷 Empregos</h3>
<p>Criação de novas oportunidades de trabalho.</p>
</div>

</div>

</section>

<section class="reveal">

<h2 class="section-title">Equipe do Projeto</h2>

<div class="people">

<div class="person">
<div class="avatar">👨‍🌾</div>
<h3>Agricultor</h3>
<p>Responsável pela propriedade.</p>
</div>

<div class="person">
<div class="avatar">👩‍🔬</div>
<h3>Engenheira Ambiental</h3>
<p>Avalia impactos ambientais.</p>
</div>

<div class="person">
<div class="avatar">👷‍♂️</div>
<h3>Técnico em Energia</h3>
<p>Instala e monitora os sistemas.</p>
</div>

</div>

</section>

<section id="planejamento" class="reveal">

<h2 class="section-title">Planejamento 5W2H</h2>

<table>

<tr>
<th>Item</th>
<th>Descrição</th>
</tr>

<tr>
<td>What</td>
<td>Implantar energia eólica na propriedade rural.</td>
</tr>

<tr>
<td>Why</td>
<td>Reduzir custos e aumentar sustentabilidade.</td>
</tr>

<tr>
<td>Where</td>
<td>Áreas rurais com potencial eólico.</td>
</tr>

<tr>
<td>When</td>
<td>Após estudo de viabilidade.</td>
</tr>

<tr>
<td>Who</td>
<td>Produtores e especialistas.</td>
</tr>

<tr>
<td>How</td>
<td>Instalação de aerogeradores.</td>
</tr>

<tr>
<td>How Much</td>
<td>Conforme porte do projeto.</td>
</tr>

</table>

</section>

<section id="grafico" class="reveal">

<h2 class="section-title">
Índice de Benefícios
</h2>

<div class="chart-container">
<canvas id="chart"></canvas>
</div>

</section>

<footer>

<h3>Energia Eólica Rural</h3>

<p>
Projeto acadêmico sobre sustentabilidade,
inovação e energias renováveis.
</p>

</footer>

<script>

const numbers =
document.querySelectorAll(".number");

numbers.forEach(num=>{

const target =
+num.getAttribute("data-target");

let count=0;

const update=()=>{

count += target/80;

if(count < target){

num.innerText =
Math.floor(count) + "%";

requestAnimationFrame(update);

}else{

num.innerText =
target + "%";
}

};

update();

});

const observer =
new IntersectionObserver(entries=>{

entries.forEach(entry=>{

if(entry.isIntersecting){

entry.target.classList.add("active");

}

});

});

document
.querySelectorAll(".reveal")
.forEach(el=>observer.observe(el));

const ctx =
document.getElementById("chart");

new Chart(ctx,{

type:"bar",

data:{

labels:[
"Economia",
"Sustentabilidade",
"Autonomia",
"Empregos",
"Valorização"
],

datasets:[{

label:"Índice (%)",

data:[
90,
95,
85,
70,
80
],

backgroundColor:[
"#FFD700",
"#FFC107",
"#FFB300",
"#FFA000",
"#FF8F00"
]

}]

},

options:{

responsive:true,

plugins:{

legend:{
display:false
}

},

scales:{

y:{
beginAtZero:true,
max:100
}

}

}

});

</script>

</body>
</html>
