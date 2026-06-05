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

body{
    background:linear-gradient(180deg,#000000,#111111,#FFD700);
    color:white;
}

header{
    min-height:100vh;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    padding:40px;
    background:
    linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.6)),
    url("https://images.unsplash.com/photo-1466611653911-95081537e5b7?auto=format&fit=crop&w=1800&q=80");
    background-size:cover;
    background-position:center;
}

.hero{
    max-width:900px;
}

.hero h1{
    font-size:4rem;
    color:#FFD700;
    margin-bottom:20px;
}

.hero p{
    font-size:1.4rem;
    line-height:1.8;
}

section{
    padding:80px 10%;
}

h2{
    color:#FFD700;
    margin-bottom:25px;
    font-size:2rem;
}

p{
    line-height:1.9;
    font-size:1.1rem;
}

.personagens{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:50px;
    margin-top:40px;
}

.personagem{
    text-align:center;
}

.personagem .icone{
    font-size:90px;
}

.personagem h3{
    color:#FFD700;
    margin-top:15px;
}

table{
    width:100%;
    margin-top:20px;
    border-collapse:collapse;
}

th{
    background:#FFD700;
    color:black;
    padding:15px;
}

td{
    padding:15px;
    border-bottom:1px solid rgba(255,255,255,.2);
}

.beneficios{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:30px;
    margin-top:30px;
}

.item{
    text-align:center;
}

.item span{
    font-size:60px;
}

canvas{
    background:white;
    border-radius:15px;
    padding:20px;
    margin-top:30px;
}

footer{
    text-align:center;
    padding:40px;
    background:black;
}

footer p{
    color:#FFD700;
}

@media(max-width:768px){

.hero h1{
    font-size:2.5rem;
}

.hero p{
    font-size:1rem;
}

section{
    padding:60px 7%;
}

}

</style>

</head>
<body>

<header>

<div class="hero">

<h1>🌬️ Energia Eólica na Zona Rural</h1>

<p>
Uma solução sustentável para reduzir custos,
promover a independência energética e fortalecer
o desenvolvimento do agronegócio brasileiro.
</p>

</div>

</header>

<section>

<h2>📖 Introdução</h2>

<p>
A energia eólica é produzida por meio da força dos ventos,
convertida em eletricidade através de aerogeradores.
No meio rural, essa tecnologia vem se tornando uma alternativa
estratégica para diminuir despesas energéticas, ampliar a
autonomia das propriedades e incentivar práticas sustentáveis.
</p>

</section>

<section>

<h2>🌎 Importância da Energia Eólica</h2>

<div class="beneficios">

<div class="item">
<span>💰</span>
<h3>Economia</h3>
<p>Redução significativa dos custos com energia elétrica.</p>
</div>

<div class="item">
<span>🌱</span>
<h3>Sustentabilidade</h3>
<p>Fonte limpa, renovável e com baixa emissão de poluentes.</p>
</div>

<div class="item">
<span>⚡</span>
<h3>Autonomia</h3>
<p>Menor dependência da rede elétrica convencional.</p>
</div>

<div class="item">
<span>👷</span>
<h3>Empregos</h3>
<p>Geração de oportunidades na instalação e manutenção.</p>
</div>

</div>

</section>

<section>

<h2>👨‍🌾 Personagens do Projeto</h2>

<div class="personagens">

<div class="personagem">
<div class="icone">👨‍🌾</div>
<h3>Agricultor</h3>
<p>Responsável pela propriedade rural.</p>
</div>

<div class="personagem">
<div class="icone">👩‍🔬</div>
<h3>Engenheira Ambiental</h3>
<p>Avalia impactos e sustentabilidade.</p>
</div>

<div class="personagem">
<div class="icone">👷‍♂️</div>
<h3>Técnico em Energia</h3>
<p>Instala e realiza manutenção dos equipamentos.</p>
</div>

</div>

</section>

<section>

<h2>📋 Planejamento 5W2H</h2>

<table>

<tr>
<th>Elemento</th>
<th>Descrição</th>
</tr>

<tr>
<td>What</td>
<td>Implantar um sistema de geração de energia eólica.</td>
</tr>

<tr>
<td>Why</td>
<td>Reduzir custos, aumentar a sustentabilidade e a autonomia.</td>
</tr>

<tr>
<td>Where</td>
<td>Propriedades rurais com potencial eólico adequado.</td>
</tr>

<tr>
<td>When</td>
<td>Após estudos de viabilidade técnica e econômica.</td>
</tr>

<tr>
<td>Who</td>
<td>Produtores rurais, engenheiros e empresas especializadas.</td>
</tr>

<tr>
<td>How</td>
<td>Instalação de aerogeradores e integração à rede elétrica.</td>
</tr>

<tr>
<td>How Much</td>
<td>Investimento variável conforme porte do projeto.</td>
</tr>

</table>

</section>

<section>

<h2>📊 Índice de Benefícios da Energia Eólica</h2>

<canvas id="grafico"></canvas>

</section>

<section>

<h2>✅ Conclusão</h2>

<p>
A implementação da energia eólica no meio rural representa uma
importante oportunidade para modernizar propriedades agrícolas,
reduzir custos operacionais e contribuir para a preservação do meio
ambiente. Com planejamento adequado e análise de viabilidade,
os benefícios econômicos e ambientais podem gerar resultados
expressivos a longo prazo.
</p>

</section>

<footer>

<p>
Energia Eólica Rural • Projeto Acadêmico • 2026
</p>

</footer>

<script>

const ctx = document.getElementById('grafico');

new Chart(ctx,{
    type:'bar',
    data:{
        labels:[
            'Economia',
            'Sustentabilidade',
            'Autonomia',
            'Empregos',
            'Valorização'
        ],
        datasets:[{
            label:'Índice (%)',
            data:[90,95,85,70,80],
            backgroundColor:[
                '#FFD700',
                '#FFC107',
                '#FFB300',
                '#FFA000',
                '#FF8F00'
            ]
        }]
    },
    options:{
        responsive:true,
        plugins:{
            legend:{
                labels:{
                    color:'black'
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
