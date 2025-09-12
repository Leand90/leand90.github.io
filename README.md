<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Assista trailers de filmes de ação, aventura, romance, drama, suspense e terror. Confira os últimos lançamentos no ReelTrailers.">
<meta name="keywords" content="trailers, filmes, lançamentos, cinema, ação, aventura, romance, drama, suspense, terror">
<meta name="author" content="ReelTrailers">
<meta name="google-adsense-account" content="ca-pub-3305836590830208">
<title>ReelTrailers | Trailers de Filmes e Lançamentos</title>
<link rel="icon" type="image/x-icon" href="http://googleusercontent.com/image_generation_content/0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<style>
:root{
--bg:#121212;--text:#fff;--gold:#FFD700;
}
*{margin:0;padding:0;box-sizing:border-box;}
body{font-family:'Helvetica Neue',Arial,sans-serif;background:var(--bg);color:var(--text);}
.header{display:flex;justify-content:space-between;align-items:center;padding:15px 40px;background:#111;position:sticky;top:0;z-index:100;}
.logo{font-size:24px;font-weight:bold;color:var(--gold);display:flex;align-items:center;}
.logo i{margin-right:5px;}
.menu ul{display:flex;list-style:none;gap:20px;}
.menu a{text-decoration:none;color:white;font-size:17px;transition:0.3s;}
.menu a:hover{color:var(--gold);}
.hamburger{display:none;font-size:28px;cursor:pointer;background:none;border:none;color:white;}
@media(max-width:768px){.menu{display:none;flex-direction:column;position:absolute;top:65px;left:0;width:100%;background:#111;padding:20px 0;}
.menu.active{display:flex;}
.menu ul{flex-direction:column;gap:15px;text-align:center;}
.hamburger{display:block;}}

/* Categoria */
.category-section{margin:40px 20px;position:relative;}
.category-header{font-size:28px;margin-bottom:15px;font-weight:bold;}
.card-carousel{display:flex;overflow-x:auto;scroll-behavior:smooth;gap:15px;}
.card-carousel::-webkit-scrollbar{display:none;}
.card{position:relative;width:200px;height:300px;flex-shrink:0;border-radius:10px;overflow:hidden;cursor:pointer;transition:transform 0.3s;}
.card img{width:100%;height:100%;object-fit:cover;display:block;}
.card-overlay{position:absolute;bottom:0;left:0;width:100%;height:100%;background:rgba(0,0,0,0.7);display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;opacity:0;padding:15px;transition:opacity 0.3s;}
.card h3{margin-bottom:10px;font-size:0.9em;font-weight:bold;}
.card p{font-size:0.8em;line-height:1.2em;}
.card:hover{transform:scale(1.1);}
.card:hover .card-overlay{opacity:1;}
.card video{width:100%;height:100%;object-fit:cover;display:none;position:absolute;top:0;left:0;z-index:-1;}

/* Botões carrossel */
.carousel-button{position:absolute;top:50%;transform:translateY(-50%);background:rgba(0,0,0,0.6);border:none;font-size:30px;color:white;cursor:pointer;z-index:10;padding:5px 10px;border-radius:50%;}
.prev-button{left:-10px;} .next-button{right:-10px;}

/* Modal */
.video-modal{display:none;position:fixed;top:0;left:0;width:100%;height:100%;background:rgba(20,20,20,0.95);justify-content:center;align-items:center;z-index:1000;}
.video-modal-content{position:relative;width:90%;max-width:900px;aspect-ratio:16/9;background:#000;border-radius:10px;overflow:hidden;}
.video-modal iframe{width:100%;height:100%;border:none;}
.modal-close-btn{position:absolute;top:-50px;right:0;color:white;font-size:2em;cursor:pointer;}
</style>
</head>
<body>

<header class="header">
<div class="logo"><i class="fab fa-youtube"></i> ReelTrailers</div>
<button class="hamburger"><i class="fas fa-bars"></i></button>
<nav class="menu">
<ul>
<li><a href="#lancamentos">Lançamentos</a></li>
<li><a href="#acao">Ação</a></li>
<li><a href="#aventura">Aventura</a></li>
<li><a href="#romance">Romance</a></li>
<li><a href="#ficcao">Ficção</a></li>
<li><a href="#comedia">Comédia</a></li>
<li><a href="#terror">Terror</a></li>
<li><a href="#anime">Anime</a></li>
</ul>
</nav>
</header>

<main>
<section id="lancamentos" class="category-section">
<h2 class="category-header">Lançamentos</h2>
<button class="carousel-button prev-button" data-container="lancamentos-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="lancamentos-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="lancamentos-carousel"></div>
</section>

<section id="acao" class="category-section">
<h2 class="category-header">Ação</h2>
<button class="carousel-button prev-button" data-container="acao-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="acao-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="acao-carousel"></div>
</section>

<section id="aventura" class="category-section">
<h2 class="category-header">Aventura</h2>
<button class="carousel-button prev-button" data-container="aventura-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="aventura-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="aventura-carousel"></div>
</section>

<section id="romance" class="category-section">
<h2 class="category-header">Romance</h2>
<button class="carousel-button prev-button" data-container="romance-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="romance-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="romance-carousel"></div>
</section>

<section id="ficcao" class="category-section">
<h2 class="category-header">Ficção</h2>
<button class="carousel-button prev-button" data-container="ficcao-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="ficcao-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="ficcao-carousel"></div>
</section>

<section id="comedia" class="category-section">
<h2 class="category-header">Comédia</h2>
<button class="carousel-button prev-button" data-container="comedia-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="comedia-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="comedia-carousel"></div>
</section>

<section id="terror" class="category-section">
<h2 class="category-header">Terror</h2>
<button class="carousel-button prev-button" data-container="terror-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="terror-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="terror-carousel"></div>
</section>

<section id="anime" class="category-section">
<h2 class="category-header">Anime</h2>
<button class="carousel-button prev-button" data-container="anime-carousel"><i class="fas fa-chevron-left"></i></button>
<button class="carousel-button next-button" data-container="anime-carousel"><i class="fas fa-chevron-right"></i></button>
<div class="card-carousel" id="anime-carousel"></div>
</section>
</main>

<div class="video-modal" id="video-modal">
<div class="video-modal-content">
<i class="fas fa-times modal-close-btn"></i>
<iframe id="video-frame" src="" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>
</div>

<script>
const API_KEY = "23d2fcca011bbb4e5f88ba16f9bede18";
const categories = {lancamentos:"upcoming",acao:28,aventura:12,romance:10749,ficcao:878,comedia:35,terror:27,anime:16};

const hamburger = document.querySelector('.hamburger');
const menu = document.querySelector('.menu');
hamburger.addEventListener('click',()=>menu.classList.toggle('active'));

async function getTrailer(movie_id){
const res = await fetch(`https://api.themoviedb.org/3/movie/${movie_id}/videos?api_key=${API_KEY}&language=pt-BR`);
const data = await res.json();
const trailer = data.results.find(v=>v.type==="Trailer" && v.site==="YouTube");
return trailer?`https://www.youtube.com/embed/${trailer.key}?autoplay=1&mute=1&controls=0`:"";
}

function createCard(movie,trailerUrl){
let overview = movie.overview?movie.overview.substring(0,80)+"...":"";
return `<div class="card">
<img src="https://image.tmdb.org/t/p/w500${movie.poster_path}" alt="${movie.title}">
<video src="${trailerUrl}" muted loop></video>
<div class="card-overlay"><h3>${movie.title}</h3><p>${overview}</p></div>
</div>`;
}

async function loadCategory(cat,containerId){
let url = cat==="lancamentos"?`https://api.themoviedb.org/3/movie/upcoming?api_key=${API_KEY}&language=pt-BR`
:`https://api.themoviedb.org/3/discover/movie?api_key=${API_KEY}&with_genres=${categories[cat]}&language=pt-BR`;
const res = await fetch(url);
const data = await res.json();
const container = document.getElementById(containerId);
container.innerHTML="";
for(let movie of data.results){
let trailerUrl = await getTrailer(movie.id);
container.innerHTML+=createCard(movie,trailerUrl);
}
container.querySelectorAll(".card").forEach(card=>{
const video = card.querySelector("video");
card.addEventListener("mouseenter",()=>{if(video){video.style.display="block";video.play();}});
card.addEventListener("mouseleave",()=>{if(video){video.pause();video.style.display="none";}});
card.addEventListener("click",()=>{openVideo(video.src);});
});
}

function setupCarouselButtons(){
document.querySelectorAll(".next-button").forEach(btn=>{btn.addEventListener('click',()=>{const container=document.getElementById(btn.dataset.container);container.scrollBy({left:300,behavior:'smooth'});});});
document.querySelectorAll(".prev-button").forEach(btn=>{btn.addEventListener('click',()=>{const container=document.getElementById(btn.dataset.container);container.scrollBy({left:-300,behavior:'smooth'});});});
}

async function loadAll(){
for(let cat in categories){await loadCategory(cat,`${cat}-carousel`);}
setupCarouselButtons();
}
loadAll();

const modal = document.getElementById("video-modal");
const frame = document.getElementById("video-frame");
document.querySelector(".modal-close-btn").addEventListener("click",()=>{modal.style.display="none";frame.src="";});
function openVideo(url){modal.style.display="flex";frame.src=url;}
</script>
</body>
</html>
