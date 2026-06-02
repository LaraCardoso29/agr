<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Energia Eólica na Zona Rural</title>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
}

body{
    background:linear-gradient(135deg,#FFE082,#FFF8E1);
    color:#333;
}

/* CABEÇALHO */
header{
    text-align:center;
    padding:40px 20px;
    background:linear-gradient(90deg,#2E7D32,#43A047);
    color:white;
}

header h1{
    font-size:40px;
}

header p{
    margin-top:10px;
}

/* IMAGEM PRINCIPAL */
.hero{
    width:100%;
    height:350px;
    overflow:hidden;
}

.hero img{
    width:100%;
    height:100%;
    object-fit:cover;
}

/* CONTAINER */
.container{
    width:90%;
    max-width:1100px;
    margin:auto;
    padding:30px 0;
}

/* CARD */
.card{
    background:white;
    padding:25px;
    margin-bottom:20px;
    border-radius:15px;
    box-shadow:0 6px 18px rgba(0,0,0,0.12);
    border-left:6px solid #43A047;
}

/* TITULOS */
h2{
    color:#2E7D32;
    margin-bottom:15px;
}

/* TABELA */
table{
    width:100%;
    border-collapse:collapse;
}

th{
    background:#43A047;
    color:white;
    padding:12px;
}

td{
    border:1px solid #ddd;
    padding:12px;
}

/* CATAVENTOS */
.area-cataventos{
    display:flex;
    justify-content:center;
    gap:40px;
    margin:40px 0;
}

.catavento{
    position:relative;
    width:100px;
    height:150px;
}

.helice{
    width:100px;
    height:100px;
    position:absolute;
    animation:girar 4s linear infinite;
}

.pala{
    position:absolute;
    width:18px;
    height:50px;
    background:#4CAF50;
    border-radius:10px;
    left:41px;
}

.p1{transform:rotate(0deg);}
.p2{transform:rotate(90deg);}
.p3{transform:rotate(180deg);}
.p4{transform:rotate(270deg);}

.centro{
    position:absolute;
    width:16px;
    height:16px;
    background:#333;
    border-radius:50%;
    top:42px;
    left:42px;
}

.torre{
    position:absolute;
    width:6px;
    height:90px;
    background:#555;
    left:47px;
    top:60px;
}

@keyframes girar{
    from{transform:rotate(0deg);}
    to{transform:rotate(360deg);}
}

/* GALERIA */
.galeria{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:15px;
}

.galeria img{
    width:100%;
    height:180px;
    object-fit:cover;
    border-radius:12px;
}

/* FOOTER */
footer{
    text-align:center;
    padding:20px;
    background:#2E7D32;
    color:white;
    margin-top:30px;
}

</style>
</head>

<body>

<header>
    <h1>🌬 Energia Eólica na Zona Rural</h1>
    <p>Projeto sustentável de geração de energia limpa</p>
</header>

<!-- IMAGEM PRINCIPAL -->
<div class="hero">
    <img src="https://images.unsplash.com/photo-1466611653911-95081537e5b7" alt="Energia Eólica">
</div>

<div class="container">

<!-- CATAVENTOS -->
<div class="area-cataventos">

    <div class="catavento">
        <div class="helice">
            <div class="pala p1"></div>
            <div class="pala p2"></div>
            <div class="pala p3"></div>
            <div class="pala p4"></div>
        </div>
        <div class="centro"></div>
        <div class="torre"></div>
    </div>

    <div class="catavento">
        <div class="helice">
            <div class="pala p1"></div>
            <div class="pala p2"></div>
            <div class="pala p3"></div>
            <div class="pala p4"></div>
        </div>
        <div class="centro"></div>
        <div class="torre"></div>
    </div>

    <div class="catavento">
        <div class="helice">
            <div class="pala p1"></div>
            <div class="pala p2"></div>
            <div class="pala p3"></div>
            <div class="pala p4"></div>
        </div>
        <div class="centro"></div>
        <div class="torre"></div>
    </div>

</div>

<!-- INTRO -->
<div class="card">
<h2>O que é Energia Eólica?</h2>
<p>
A energia eólica utiliza a força dos ventos para gerar eletricidade através de aerogeradores.
É uma fonte limpa, renovável e muito usada em áreas rurais.
</p>
</div>

<!-- BENEFICIOS -->
<div class="card">
<h2>Benefícios</h2>
<ul>
<li>Energia limpa e renovável</li>
<li>Redução de custos</li>
<li>Baixo impacto ambiental</li>
<li>Independência energética</li>
<li>Sustentabilidade no campo</li>
</ul>
</div>

<!-- GALERIA -->
<div class="card">
<h2>Imagens da Energia Eólica</h2>

<div class="galeria">

<img src="https://images.unsplash.com/photo-1509391366360-2e959784a276">
<img src="https://images.unsplash.com/photo-1508514177221-188b1cf16e9d">
<img src="https://images.unsplash.com/photo-1509395176047-4a66953fd231">

</div>

</div>

<!-- 5W2H -->
<div class="card">
<h2>Pesquisa 5W2H</h2>

<table>

<tr><th>Item</th><th>Descrição</th></tr>

<tr><td>What</td><td>Implementação de energia eólica na zona rural</td></tr>
<tr><td>Why</td><td>Reduzir custos e poluição</td></tr>
<tr><td>Where</td><td>Áreas rurais</td></tr>
<tr><td>When</td><td>Após estudo técnico</td></tr>
<tr><td>Who</td><td>Engenheiros e produtores</td></tr>
<tr><td>How</td><td>Instalação de turbinas eólicas</td></tr>
<tr><td>How Much</td><td>Depende do projeto</td></tr>

</table>

</div>

<!-- CONCLUSÃO -->
<div class="card">
<h2>Conclusão</h2>
<p>
A energia eólica é uma solução sustentável que reduz impactos ambientais
e melhora a economia no campo.
</p>
</div>

</div>

<footer>
Projeto Escolar • Energia Eólica na Zona Rural
</footer>

</body>
</html>
