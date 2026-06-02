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
    background:linear-gradient(135deg,#FFE082,#FFF3C4);
    color:#333;
}

/* CABEÇALHO */
header{
    text-align:center;
    padding:40px 20px;
    background:linear-gradient(90deg,#2E7D32,#43A047);
    color:white;
    box-shadow:0 4px 10px rgba(0,0,0,0.2);
}

header h1{
    font-size:38px;
}

header p{
    margin-top:10px;
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
    transition:0.3s;
    border-left:6px solid #43A047;
}

.card:hover{
    transform:translateY(-5px);
}

h2{
    color:#2E7D32;
    margin-bottom:15px;
}

p, td{
    line-height:1.6;
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
    height:160px;
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
    transform-origin:center 50px;
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

/* RESPONSIVO */
@media(max-width:700px){
    .area-cataventos{
        flex-direction:column;
        align-items:center;
    }
}

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
    <p>Pesquisa 5W2H sobre energia limpa e sustentável</p>
</header>

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

<!-- SOBRE -->
<div class="card">
    <h2>O que é Energia Eólica?</h2>
    <p>
        A energia eólica é gerada pela força dos ventos, que movimenta turbinas
        capazes de produzir eletricidade de forma limpa e sustentável. Na zona rural,
        ela reduz custos e aumenta a autonomia energética.
    </p>
</div>

<!-- 5W2H -->
<div class="card">
    <h2>Pesquisa 5W2H</h2>

    <table>
        <tr>
            <th>Item</th>
            <th>Descrição</th>
        </tr>

        <tr>
            <td><b>What (O quê?)</b></td>
            <td>Implementação de energia eólica na zona rural</td>
        </tr>

        <tr>
            <td><b>Why (Por quê?)</b></td>
            <td>Reduzir custos e promover sustentabilidade ambiental</td>
        </tr>

        <tr>
            <td><b>Where (Onde?)</b></td>
            <td>Áreas rurais com potencial de vento</td>
        </tr>

        <tr>
            <td><b>When (Quando?)</b></td>
            <td>Após análise de viabilidade técnica</td>
        </tr>

        <tr>
            <td><b>Who (Quem?)</b></td>
            <td>Produtores rurais, engenheiros e empresas do setor</td>
        </tr>

        <tr>
            <td><b>How (Como?)</b></td>
            <td>Instalação de aerogeradores conectados ao sistema elétrico</td>
        </tr>

        <tr>
            <td><b>How Much (Quanto custa?)</b></td>
            <td>Depende do tamanho do projeto e infraestrutura necessária</td>
        </tr>

    </table>
</div>

<!-- CONCLUSÃO -->
<div class="card">
    <h2>Conclusão</h2>
    <p>
        A energia eólica é uma solução sustentável e eficiente para o meio rural,
        promovendo economia, autonomia energética e preservação do meio ambiente.
    </p>
</div>

</div>

<footer>
Projeto Escolar • Energia Eólica na Zona Rural
</footer>

</body>
</html>
