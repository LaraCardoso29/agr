<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Dashboard - Energia Eólica na Zona Rural</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
}

body{
    display:flex;
    min-height:100vh;
    background:#f5f7f2;
}

/* MENU LATERAL */
.sidebar{
    width:260px;
    background:linear-gradient(180deg,#2E7D32,#43A047);
    color:white;
    padding:20px;
}

.sidebar h2{
    text-align:center;
    margin-bottom:30px;
}

.menu button{
    width:100%;
    padding:12px;
    margin-bottom:10px;
    border:none;
    border-radius:10px;
    cursor:pointer;
    font-weight:bold;
    background:rgba(255,255,255,0.15);
    color:white;
    transition:0.3s;
}

.menu button:hover{
    background:rgba(255,255,255,0.3);
}

/* CONTEÚDO */
.content{
    flex:1;
    padding:25px;
}

/* SEÇÕES */
.section{
    display:none;
    animation:fade 0.4s ease-in-out;
}

.active{
    display:block;
}

@keyframes fade{
    from{opacity:0; transform:translateY(10px);}
    to{opacity:1; transform:translateY(0);}
}

/* CARDS */
.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:15px;
    margin-bottom:20px;
}

.card{
    background:white;
    padding:20px;
    border-radius:15px;
    box-shadow:0 5px 15px rgba(0,0,0,0.1);
    text-align:center;
    border-top:4px solid #43A047;
}

.numero{
    font-size:28px;
    font-weight:bold;
    color:#F9A825;
    margin-top:10px;
}

/* TABELA */
table{
    width:100%;
    border-collapse:collapse;
    background:white;
    border-radius:10px;
    overflow:hidden;
}

th{
    background:#43A047;
    color:white;
    padding:10px;
}

td{
    border:1px solid #ddd;
    padding:10px;
}

/* GRAFICOS */
.graficos{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

canvas{
    background:white;
    padding:10px;
    border-radius:10px;
}

/* RESPONSIVO */
@media(max-width:900px){
    .sidebar{
        width:200px;
    }
    .graficos{
        grid-template-columns:1fr;
    }
}

</style>
</head>

<body>

<!-- MENU -->
<div class="sidebar">
<h2>🌬 Energia Eólica</h2>

<div class="menu">
<button onclick="mostrar('inicio')">Início</button>
<button onclick="mostrar('indicadores')">Indicadores</button>
<button onclick="mostrar('graficos')">Gráficos</button>
<button onclick="mostrar('cinco')">5W2H</button>
<button onclick="mostrar('conclusao')">Conclusão</button>
</div>
</div>

<!-- CONTEÚDO -->
<div class="content">

<!-- INICIO -->
<div id="inicio" class="section active">
<h1>🌾 Energia Eólica na Zona Rural</h1>
<br>
<p>
Este painel apresenta um estudo sobre a implementação da energia eólica na zona rural,
abordando viabilidade, impacto ambiental e benefícios econômicos.
</p>
</div>

<!-- INDICADORES -->
<div id="indicadores" class="section">

<h2>Indicadores</h2>
<br>

<div class="cards">

<div class="card">
<h3>Economia</h3>
<div class="numero">35%</div>
</div>

<div class="card">
<h3>CO₂ Reduzido</h3>
<div class="numero">25t/ano</div>
</div>

<div class="card">
<h3>Retorno</h3>
<div class="numero">6 anos</div>
</div>

<div class="card">
<h3>Eficiência</h3>
<div class="numero">95%</div>
</div>

</div>

</div>

<!-- GRAFICOS -->
<div id="graficos" class="section">

<h2>Gráficos de Análise</h2>
<br>

<div class="graficos">

<canvas id="grafico1"></canvas>
<canvas id="grafico2"></canvas>

</div>

</div>

<!-- 5W2H -->
<div id="cinco" class="section">

<h2>Pesquisa 5W2H</h2>
<br>

<table>
<tr><th>Item</th><th>Descrição</th></tr>
<tr><td>What</td><td>Energia eólica na zona rural</td></tr>
<tr><td>Why</td><td>Reduzir custos e impacto ambiental</td></tr>
<tr><td>Where</td><td>Propriedades rurais</td></tr>
<tr><td>When</td><td>Após estudo técnico</td></tr>
<tr><td>Who</td><td>Engenheiros e produtores</td></tr>
<tr><td>How</td><td>Instalação de aerogeradores</td></tr>
<tr><td>How Much</td><td>Depende do projeto</td></tr>
</table>

</div>

<!-- CONCLUSÃO -->
<div id="conclusao" class="section">

<h2>Conclusão</h2>
<br>

<p>
A energia eólica é uma alternativa sustentável e eficiente para o meio rural,
promovendo economia, autonomia energética e preservação ambiental.
</p>

</div>

</div>

<script>

/* MENU */
function mostrar(id){

    let secoes = document.querySelectorAll('.section');
    secoes.forEach(s => s.classList.remove('active'));

    document.getElementById(id).classList.add('active');
}

/* GRAFICO 1 */
new Chart(document.getElementById('grafico1'),{
type:'bar',
data:{
labels:['Ano 1','Ano 2','Ano 3','Ano 4','Ano 5'],
datasets:[{
label:'Economia (R$)',
data:[4000,6000,9000,11000,14000],
backgroundColor:'#43A047'
}]
}
});

/* GRAFICO 2 */
new Chart(document.getElementById('grafico2'),{
type:'doughnut',
data:{
labels:['Eólica','Solar','Hidrelétrica','Petróleo','Carvão'],
datasets:[{
data:[5,10,20,35,30],
backgroundColor:['#43A047','#FDD835','#1E88E5','#FB8C00','#424242']
}]
}
});

</script>

</body>
</html>
