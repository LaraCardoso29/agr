<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Energia Eólica na Zona Rural</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
}

/* FUNDO */
body{
    background:linear-gradient(135deg,#FFE082,#FFF3C4);
    color:#333;
}

/* TELA INICIAL */
#intro{
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
    text-align:center;
    background:linear-gradient(135deg,#2E7D32,#66BB6A);
    color:white;
}

#intro h1{
    font-size:48px;
    margin-bottom:15px;
}

#intro p{
    font-size:18px;
    max-width:600px;
    margin-bottom:30px;
}

button{
    padding:15px 30px;
    font-size:18px;
    border:none;
    border-radius:30px;
    cursor:pointer;
    background:#FFD54F;
    color:#333;
    font-weight:bold;
    transition:0.3s;
}

button:hover{
    transform:scale(1.05);
}

/* DASHBOARD */
#dashboard{
    display:none;
}

/* HEADER */
header{
    background:linear-gradient(90deg,#2E7D32,#43A047);
    color:white;
    text-align:center;
    padding:30px;
}

header h1{
    font-size:38px;
}

/* CONTAINER */
.container{
    width:90%;
    max-width:1200px;
    margin:auto;
    padding:25px 0;
}

/* CARDS */
.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
    gap:20px;
    margin-bottom:25px;
}

.card{
    background:white;
    padding:20px;
    border-radius:15px;
    text-align:center;
    box-shadow:0 8px 20px rgba(0,0,0,0.12);
    border-top:5px solid #43A047;
}

.card h3{
    color:#2E7D32;
}

.numero{
    font-size:32px;
    font-weight:bold;
    color:#F9A825;
    margin-top:10px;
}

/* SEÇÕES */
.section{
    background:white;
    padding:20px;
    border-radius:15px;
    margin-bottom:20px;
    box-shadow:0 6px 18px rgba(0,0,0,0.1);
}

.section h2{
    color:#2E7D32;
    margin-bottom:15px;
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
    border-radius:15px;
}

/* TABELA */
table{
    width:100%;
    border-collapse:collapse;
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

/* RESPONSIVO */
@media(max-width:900px){
    .graficos{
        grid-template-columns:1fr;
    }
}

</style>
</head>

<body>

<!-- INTRO -->
<div id="intro">
    <h1>🌬 Energia Eólica</h1>
    <p>Projeto sobre implementação de energia eólica na zona rural com gráficos, indicadores e análise 5W2H.</p>
    <button id="btnIniciar">Iniciar Projeto</button>
</div>

<!-- DASHBOARD -->
<div id="dashboard">

<header>
    <h1>Implementação da Energia Eólica na Zona Rural</h1>
</header>

<div class="container">

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

<div class="section">
<h2>Introdução</h2>
<p>
A energia eólica é uma fonte renovável que utiliza a força dos ventos para gerar eletricidade,
promovendo sustentabilidade e redução de custos na zona rural.
</p>
</div>

<div class="graficos">

<div class="section">
<h2>Economia ao Longo dos Anos</h2>
<canvas id="grafico1"></canvas>
</div>

<div class="section">
<h2>Impacto Ambiental</h2>
<canvas id="grafico2"></canvas>
</div>

</div>

<div class="section">

<h2>Pesquisa 5W2H</h2>

<table>
<tr><th>Item</th><th>Descrição</th></tr>
<tr><td>What</td><td>Energia eólica na zona rural</td></tr>
<tr><td>Why</td><td>Reduzir custos e impacto ambiental</td></tr>
<tr><td>Where</td><td>Áreas rurais</td></tr>
<tr><td>When</td><td>Após estudo técnico</td></tr>
<tr><td>Who</td><td>Engenheiros e produtores</td></tr>
<tr><td>How</td><td>Instalação de aerogeradores</td></tr>
<tr><td>How Much</td><td>Depende do projeto</td></tr>
</table>

</div>

<div class="section">
<h2>Conclusão</h2>
<p>
A energia eólica é uma solução sustentável e eficiente para o meio rural,
trazendo economia e preservação ambiental.
</p>
</div>

</div>
</div>

<script>

/* BOTÃO FUNCIONANDO */
document.getElementById("btnIniciar").addEventListener("click", function(){
    document.getElementById("intro").style.display = "none";
    document.getElementById("dashboard").style.display = "block";
});

/* GRÁFICO 1 */
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

/* GRÁFICO 2 */
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



