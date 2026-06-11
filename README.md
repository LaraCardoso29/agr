<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Energia Eólica na Zona Rural</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>

<style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:linear-gradient(
        135deg,
        #022c22 0%,
        #064e3b 30%,
        #065f46 60%,
        #022c22 100%
    );

    color:white;
    overflow-x:hidden;
}

header{
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;

    display:flex;
    justify-content:space-between;
    align-items:center;

    padding:20px 50px;

    background:rgba(255,255,255,0.08);
    backdrop-filter:blur(15px);
}

header h1{
    font-size:28px;
}

#pesquisa{
    padding:12px;
    border:none;
    border-radius:10px;
    width:280px;
}

.hero{
    height:100vh;

    background:
    linear-gradient(
        rgba(0,0,0,.5),
        rgba(0,0,0,.5)
    ),
    url("https://images.unsplash.com/photo-1466611653911-95081537e5b7");

    background-size:cover;
    background-position:center;

    display:flex;
    justify-content:center;
    align-items:center;
    text-align:center;
}

.overlay{
    background:rgba(0,0,0,.4);
    backdrop-filter:blur(8px);

    padding:50px;
    border-radius:25px;
}

.overlay h2{
    font-size:60px;
    margin-bottom:20px;
}

.overlay p{
    font-size:22px;
}

section{
    padding:80px 10%;
}

h2{
    text-align:center;
    margin-bottom:40px;
    font-size:40px;
}

.sobre p,
.pesquisa p{
    line-height:1.8;
    font-size:18px;
    text-align:justify;
}

.cards{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:25px;
}

.card{
    width:300px;

    background:rgba(255,255,255,0.08);
    backdrop-filter:blur(15px);

    border:1px solid rgba(255,255,255,0.1);

    padding:30px;
    border-radius:20px;

    transition:.4s;
}

.card:hover{
    transform:translateY(-10px);
    box-shadow:0 15px 30px rgba(0,0,0,.4);
}

.card h3{
    margin-bottom:15px;
    color:#6ee7b7;
}

.video{
    text-align:center;
}

.video iframe{
    width:100%;
    max-width:1000px;
    height:550px;
    border:none;
    border-radius:20px;
}

table{
    width:100%;
    border-collapse:collapse;

    background:rgba(255,255,255,0.08);
    backdrop-filter:blur(12px);

    border-radius:20px;
    overflow:hidden;
}

th{
    background:#10b981;
}

td,th{
    padding:15px;
    border:1px solid rgba(255,255,255,.1);
}

.grafico{
    max-width:1000px;
    margin:auto;
}

footer{
    margin-top:80px;

    background:rgba(0,0,0,.3);

    padding:30px;
    text-align:center;
}

canvas{
    background:white;
    border-radius:20px;
    padding:20px;
}

@media(max-width:768px){

header{
    flex-direction:column;
    gap:15px;
}

.overlay h2{
    font-size:35px;
}

.cards{
    flex-direction:column;
    align-items:center;
}

.video iframe{
    height:300px;
}
}

</style>
</head>

<body>

<header>

<h1>🌿 Energia Eólica Rural</h1>

<input
type="text"
id="pesquisa"
placeholder="Pesquisar conteúdo..."
>

</header>

<section class="hero">

<div class="overlay">
<h2>Energia Eólica na Zona Rural</h2>

<p>
Sustentabilidade, economia e independência energética para o campo.
</p>

</div>

</section>

<section class="sobre">

<h2>O que é Energia Eólica?</h2>

<p>
A energia eólica é produzida pela força dos ventos por meio de aerogeradores.
Ela representa uma das principais fontes renováveis de energia do mundo,
contribuindo para a redução das emissões de gases do efeito estufa e para o
desenvolvimento sustentável das propriedades rurais.
</p>

</section>

<section class="beneficios">

<h2>Benefícios da Implantação</h2>

<div class="cards">

<div class="card">
<h3>💰 Economia</h3>
<p>
Redução significativa dos custos com energia elétrica.
</p>
</div>

<div class="card">
<h3>🌱 Sustentabilidade</h3>
<p>
Fonte limpa e renovável sem emissão de poluentes.
</p>
</div>

<div class="card">
<h3>⚡ Autonomia</h3>
<p>
Menor dependência da rede elétrica convencional.
</p>
</div>

<div class="card">
<h3>📈 Valorização</h3>
<p>
Aumento do valor da propriedade rural.
</p>
</div>

</div>

</section>

<section class="video">

<h2>Vídeo Explicativo</h2>

<iframe
src="https://www.youtube.com/embed/AbxHoQF4ADk"
allowfullscreen>
</iframe>

</section>

<section class="w2h">

<h2>Plano de Ação 5W2H</h2>

<table>

<tr>
<th>Elemento</th>
<th>Descrição</th>
</tr>

<tr>
<td>What</td>
<td>Implantar sistema de geração de energia eólica.</td>
</tr>

<tr>
<td>Why</td>
<td>Reduzir custos e promover sustentabilidade.</td>
</tr>

<tr>
<td>Where</td>
<td>Propriedades rurais com potencial de ventos.</td>
</tr>

<tr>
<td>When</td>
<td>Execução entre 6 e 12 meses.</td>
</tr>

<tr>
<td>Who</td>
<td>Produtores rurais, engenheiros e empresas especializadas.</td>
</tr>

<tr>
<td>How</td>
<td>Estudo dos ventos, licenciamento, instalação e monitoramento.</td>
</tr>

<tr>
<td>How Much</td>
<td>Investimento estimado entre R$150.000 e R$500.000.</td>
</tr>

</table>

</section>

<section class="grafico">

<h2>Impactos Esperados</h2>

<canvas id="graficoEnergia"></canvas>

</section>

<section class="pesquisa">

<h2>Pesquisa Completa</h2>

<p>
A implementação da energia eólica na zona rural permite aproveitar recursos
naturais disponíveis para geração de energia limpa e renovável. Em áreas com
ventos constantes, pequenos e médios aerogeradores podem abastecer residências,
sistemas de irrigação, galpões agrícolas e equipamentos produtivos.
</p>

<br>

<p>
Entre os benefícios observados estão a redução dos gastos com eletricidade,
maior independência energética, diminuição das emissões de carbono e valorização
da propriedade rural. Além disso, a energia eólica auxilia na diversificação da
matriz energética nacional.
</p>

<br>

<p>
Os principais desafios incluem o investimento inicial elevado, necessidade de
estudos de viabilidade, análise dos ventos, licenciamento ambiental e manutenção
dos equipamentos. Apesar disso, o retorno financeiro pode ser alcançado em médio
prazo devido à economia gerada.
</p>

</section>

<footer>

<h3>Projeto Acadêmico - Energia Eólica na Zona Rural</h3>

<p>
Desenvolvido em HTML, CSS, JavaScript e Java (Spring Boot)
</p>

</footer>

<script>

const pesquisa = document.getElementById("pesquisa");

pesquisa.addEventListener("keyup",function(){

let texto = pesquisa.value.toLowerCase();

document.querySelectorAll("section").forEach(sec=>{

if(sec.innerText.toLowerCase().includes(texto)){
sec.style.display="block";
}else{
sec.style.display="none";
}

});

});

const ctx = document.getElementById('graficoEnergia');

new Chart(ctx,{
    type:'bar',

    data:{
        labels:[
            'Economia',
            'Redução CO₂',
            'Autonomia',
            'Sustentabilidade',
            'Valorização'
        ],

        datasets:[{
            label:'Impacto (%)',

            data:[
                70,
                85,
                60,
                95,
                75
            ],

            backgroundColor:[
                '#10b981',
                '#34d399',
                '#059669',
                '#6ee7b7',
                '#047857'
            ],

            borderRadius:12
        }]
    },

    options:{
        responsive:true,

        plugins:{
            legend:{
                labels:{
                    color:'#000'
                }
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
<section class="galeria">

<h2>Parques Eólicos no Brasil</h2>

<div class="galeria-grid">

<img src="https://images.unsplash.com/photo-1466611653911-95081537e5b7">
<img src="https://images.unsplash.com/photo-1473341304170-971dccb5ac1e">
<img src="https://images.unsplash.com/photo-1509391366360-2e959784a276">
<img src="https://images.unsplash.com/photo-1497436072909-60f360e1d4b1">

</div>

</section>
<section>

<h2>✅ Vantagens da Energia Eólica</h2>

<div class="cards">

<div class="card">
<h3>Energia Renovável</h3>
<p>O vento é um recurso natural inesgotável.</p>
</div>

<div class="card">
<h3>Baixa Emissão de CO₂</h3>
<p>Não gera gases de efeito estufa durante a operação.</p>
</div>

<div class="card">
<h3>Economia</h3>
<p>Reduz gastos com energia elétrica a longo prazo.</p>
</div>

<div class="card">
<h3>Desenvolvimento Rural</h3>
<p>Gera empregos e renda para comunidades locais.</p>
</div>

</div>

</section>
<section>

<h2>⚠️ Desvantagens da Energia Eólica</h2>

<div class="cards">

<div class="card">
<h3>Dependência dos Ventos</h3>
<p>A produção varia conforme as condições climáticas.</p>
</div>

<div class="card">
<h3>Alto Investimento Inicial</h3>
<p>Instalação dos aerogeradores exige capital elevado.</p>
</div>

<div class="card">
<h3>Impacto na Fauna</h3>
<p>Pode afetar aves e morcegos.</p>
</div>

<div class="card">
<h3>Impacto Visual e Sonoro</h3>
<p>Alteração da paisagem e ruído das turbinas.</p>
</div>

</div>

</section>
<section>

<h2>🌎 Sustentabilidade</h2>

<p>
A energia eólica é considerada uma das fontes mais sustentáveis do mundo.
Ela não utiliza combustíveis fósseis, não emite gases poluentes durante a
geração e consome pouquíssima água quando comparada a outras formas de produção energética.
</p>

<p>
Além disso, contribui diretamente para a redução das mudanças climáticas,
promovendo o desenvolvimento sustentável no meio rural.
</p>

</section>
<section>

<h2>🇧🇷 Principais Regiões Eólicas do Brasil</h2>

<table>

<tr>
<th>Estado</th>
<th>Destaque</th>
</tr>

<tr>
<td>Rio Grande do Norte</td>
<td>Maior produtor nacional</td>
</tr>

<tr>
<td>Bahia</td>
<td>Grande potencial de expansão</td>
</tr>

<tr>
<td>Ceará</td>
<td>Pioneiro na geração eólica</td>
</tr>

<tr>
<td>Piauí</td>
<td>Complexo Lagoa dos Ventos</td>
</tr>

<tr>
<td>Maranhão</td>
<td>Complexo Delta do Maranhão</td>
</tr>

</table>

</section>


