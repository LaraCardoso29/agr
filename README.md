const menuBtn =
document.getElementById("menuBtn");

const nav =
document.getElementById("nav");

menuBtn.addEventListener("click",()=>{

nav.classList.toggle("active");

});

const themeBtn =
document.getElementById("themeToggle");

const body =
document.body;

if(localStorage.getItem("theme")==="dark"){

body.classList.add("dark");
themeBtn.textContent="☀️";

}

themeBtn.addEventListener("click",()=>{

body.classList.toggle("dark");

const dark =
body.classList.contains("dark");

localStorage.setItem(
"theme",
dark ? "dark":"light"
);

themeBtn.textContent=
dark ? "☀️":"🌙";

});

const noticias = [

{
titulo:"Energia Eólica Cresce no Campo",
descricao:"A energia dos ventos tem reduzido significativamente os custos energéticos das propriedades rurais.",
imagem:"https://images.unsplash.com/photo-1548337138-e87d889cc369?auto=format&fit=crop&w=800&q=80"
},

{
titulo:"Sustentabilidade em Alta",
descricao:"Fontes renováveis ajudam produtores a reduzir impactos ambientais.",
imagem:"https://images.unsplash.com/photo-1473341304170-971dccb5ac1e?auto=format&fit=crop&w=800&q=80"
},

{
titulo:"Autonomia Energética Rural",
descricao:"Aerogeradores permitem menor dependência da rede elétrica convencional.",
imagem:"https://images.unsplash.com/photo-1509395176047-4a66953fd231?auto=format&fit=crop&w=800&q=80"
},

{
titulo:"Empregos Verdes",
descricao:"A expansão da energia eólica gera novas oportunidades de trabalho.",
imagem:"https://images.unsplash.com/photo-1517048676732-d65bc937f952?auto=format&fit=crop&w=800&q=80"
},

{
titulo:"Tecnologia e Inovação",
descricao:"Novos sistemas aumentam a eficiência da geração de energia.",
imagem:"https://images.unsplash.com/photo-1497436072909-f5e4be5584d2?auto=format&fit=crop&w=800&q=80"
},

{
titulo:"Futuro do Agronegócio",
descricao:"A combinação entre tecnologia e sustentabilidade fortalece o campo.",
imagem:"https://images.unsplash.com/photo-1500937386664-56d1dfef3854?auto=format&fit=crop&w=800&q=80"
}

];

const container =
document.getElementById("newsContainer");

noticias.forEach(noticia=>{

container.innerHTML += `

<div class="card">

<img src="${noticia.imagem}" alt="${noticia.titulo}">

<div class="card-content">

<h3>${noticia.titulo}</h3>

<p>${noticia.descricao}</p>

</div>

</div>

`;

});








