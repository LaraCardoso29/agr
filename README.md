<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Implementação da Energia Eólica na Zona Rural</title>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

body{
    font-family:'Segoe UI',sans-serif;
    background:linear-gradient(135deg,#FFE082,#FFF8E1);
    color:#333;
}

header{
    background:linear-gradient(90deg,#2E7D32,#66BB6A);
    color:white;
    text-align:center;
    padding:40px;
    box-shadow:0 4px 10px rgba(0,0,0,.2);
}

header h1{
    font-size:42px;
}

header p{
    margin-top:10px;
    font-size:18px;
}

.container{
    width:90%;
    max-width:1300px;
    margin:auto;
    padding:30px 0;
}

.cards{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
    margin-bottom:30px;
}

.card{
    background:white;
    padding:25px;
    border-radius:15px;
    box-shadow:0 5px 15px rgba(0,0,0,.15);
    text-align:center;
    transition:.3s;
}

.card:hover{
    transform:translateY(-5px);
}

.card h2{
    color:#2E7D32;
    margin-bottom:10px;
}

.numero{
    font-size:35px;
    font-weight:bold;
    color:#F9A825;
}

.section{
    background:white;
    padding:25px;
    border-radius:15px;
    box-shadow:0 5px 15px rgba(0,0,0,.15);
    margin-bottom:25px;
}

.section h2{
    color:#2E7D32;
    margin-bottom:15px;
}

.graficos{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:20px;
}

canvas{
    background:white;
    border-radius:15px;
    padding:15px;
}

table{
    width:100%;
    border-collapse:collapse;
}

th{
    background:#43A047;
    color:white;
}

th,td{
    border:1px solid #ddd;
    padding:12px;
    text-align:left;
}

ul{
    margin-left:20px;
}

li{
    margin-bottom:10px;
}

footer{
    background:#2E7D32;
    color:white;
    text-align:center;
    padding:20px;
    margin-top:30px;
}

@media(max-width:900px){
    .graficos{
        grid-template-columns:1fr;
    }
}

</style>
</head>
<body>

<header>
    <h1>🌬 Implementação da Energia Eólica na Zona Rural</h1>
    <p>Pesquisa Técnica utilizando a metodologia 5W2H</p>
</header>

<div class="container">

<div class="cards">

    <div class="card">
        <h2>Economia de Energia</h2>
        <div class="numero">35%</div>
    </div>

    <div class="card">
        <h2>Redução de CO₂</h2>
        <div class="numero">25 t/ano</div>
    </div>

    <div class="card">
        <h2>Retorno do Investimento</h2>
        <div class="numero">6 anos</div>
    </div>

    <div class="card">
        <h2>Disponibilidade</h2>
        <div class="numero">95%</div>
    </div>

</div>

<div class="section">
    <h2>Introdução</h2>

    <p>
        A energia eólica é uma fonte renovável obtida através da força dos ventos.
        Sua aplicação na zona rural contribui para a redução dos custos energéticos,
        promove a sustentabilidade ambiental e aumenta a autonomia das propriedades
        agrícolas.
    </p>
</div>

<div class="graficos">

<div class="section">
    <h2>Economia Financeira ao Longo dos Anos</h2>
    <canvas id="graficoEconomia"></canvas>
</div>

<div class="section">
    <h2>Impacto Ambiental das Fontes de Energia</h2>
    <canvas id="graficoImpacto"></canvas>
</div>

</div>

<div class="section">

<h2>Pesquisa 5W2H</h2>

<table>

<tr>
<th>Item</th>
<th>Descrição</th>
</tr>

<tr>
<td>What (O quê?)</td>
<td>Implementar sistemas de energia eólica em propriedades rurais.</td>
</tr>

<tr>
<td>Why (Por quê?)</td>
<td>Reduzir custos energéticos e promover sustentabilidade.</td>
</tr>

<tr>
<td>Where (Onde?)</td>
<td>Regiões rurais com potencial adequado de ventos.</td>
</tr>

<tr>
<td>When (Quando?)</td>
<td>Após estudo de viabilidade técnica e econômica.</td>
</tr>

<tr>
<td>Who (Quem?)</td>
<td>Produtores rurais, engenheiros e empresas especializadas.</td>
</tr>

<tr>
<td>How (Como?)</td>
<td>Instalação de aerogeradores conectados ao sistema elétrico.</td>
</tr>

<tr>
<td>How Much (Quanto?)</td>
<td>O custo depende do tamanho da propriedade e da capacidade instalada.</td>
</tr>

</table>

</div>

<div class="section">

<h2>Objetivo</h2>

<p>
Avaliar a viabilidade da implementação da energia eólica na zona rural,
identificando benefícios econômicos, sociais e ambientais.
</p>

</div>

<div class="section">

<h2>Benefícios</h2>

<ul>
<li>Redução dos gastos com energia elétrica.</li>
<li>Fonte renovável e sustentável.</li>
<li>Diminuição da emissão de gases poluentes.</li>
<li>Maior independência energética.</li>
<li>Valorização da propriedade rural.</li>
<li>Contribuição para a preservação ambiental.</li>
</ul>

</div>

<div class="section">

<h2>Conclusão</h2>

<p>
A implementação da energia eólica representa uma solução moderna e eficiente
para o meio rural. Apesar do investimento inicial, os benefícios econômicos e
ambientais obtidos ao longo dos anos tornam essa tecnologia uma alternativa
estratégica para o desenvolvimento sustentável.
</p>

</div>

</div>

<footer>
Projeto Escolar • Energia Eólica na Zona Rural • Metodologia 5W2H
</footer>

<script>

new Chart(document.getElementById('graficoEconomia'), {
    type: 'bar',
    data: {
        labels: ['Ano 1','Ano 2','Ano 3','Ano 4','Ano 5'],
        datasets: [{
            label: 'Economia (R$)',
            data: [4000,6000,8500,10500,13000],
            backgroundColor: '#43A047'
        }]
    }
});

new Chart(document.getElementById('graficoImpacto'), {
    type: 'doughnut',
    data: {
        labels: ['Eólica','Solar','Hidrelétrica','Petróleo','Carvão'],
        datasets: [{
            data:[5,8,15,35,37],
            backgroundColor:[
                '#43A047',
                '#FDD835',
                '#1E88E5',
                '#FB8C00',
                '#424242'
            ]
        }]
    }
});

</script>

</body>
</html>
