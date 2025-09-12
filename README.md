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
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-3305836590830208" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<style>
:root{
  --bg-main:#800020;
  --card-bg:#111;
  --text-color:#fff;
  --overlay-color: rgba(0,0,0,0.7);
}
body{
  margin:0;
  font-family:Arial,sans-serif;
  background:var(--bg-main);
  color:var(--text-color);
  overflow-x:hidden;
}

/* HEADER */
.header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:15px 40px;
  background:#333;
  position:sticky;
  top:0;
  z-index:100;
}
.logo{
  color:#FFD700;
  font-size:20px;
  display:flex;
  align-items:center;
}
.logo i{margin-right:5px;}
.menu ul{
  display:flex;
  list-style:none;
  gap:20px;
  margin:0;
  padding:0;
}
.menu a{
  color:white;
  text-decoration:none;
  font-weight:500;
  font-size:16px;
  transition:0.3s;
}
.menu a:hover{color:#FFD700;}
.hamburger{
  display:none;
  font-size:28px;
  background:none;
  border:none;
  color:white;
  cursor:pointer;
}

/* MOBILE MENU */
@media(max-width:768px){
  .menu{
    display:none;
    flex-direction:column;
    position:absolute;
    top:60px;
    left:0;
    width:100%;
    background:#333;
    padding:15px 0;
  }
  .menu.active{display:flex;}
  .menu ul{flex-direction:column; gap:15px; text-align:center;}
  .hamburger{display:block;}
}

/* CATEGORY SECTION */
.category-section{
  padding:20px 40px;
}
.category-header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  margin-bottom:10px;
}
.category-header h2{color:#FFD700;}
.carousel{
  display:flex;
  overflow-x:auto;
  gap:15px;
  scroll-behavior:smooth;
}
.carousel::-webkit-scrollbar{display:none;}
.card{
  position:relative;
  width:180px;
  height:270px;
  border-radius:10px;
  overflow:hidden;
  cursor:pointer;
  flex-shrink:0;
  background:var(--card-bg);
  transition:transform 0.3s;
}
.card img{
  width:100%;
  height:100%;
  object-fit:cover;
}
.card-overlay{
  position:absolute;
  top:0;
  left:0;
  width:100%;
  height:100%;
  background:var(--overlay-color);
  display:flex;
  justify-content:center;
  align-items:center;
  text-align:center;
  opacity:0;
  padding:10px;
  transition:0.3s;
}
.card:hover{transform:translateY(-5px);}
.card:hover .card-overlay{opacity:1;}
.card-overlay p{
  font-size:14px;
  line-height:1.4;
}

/* ARROWS */
.arrow{
  background:none;
  border:none;
  font-size:30px;
  cursor:pointer;
  color:white;
  transition:0.3s;
}
.arrow:hover{color:#FFD700;}

/* VIDEO MODAL */
.video-modal{
  position:fixed;
  top:0; left:0;
  width:100%; height:100%;
  background:rgba(50,50,50,0.9);
  display:flex;
  justify-content:center;
  align-items:center;
  z-index:1000;
  display:none;
}
.video-content{
  width:80%;
  max-width:900px;
  aspect-ratio:16/9;
  background:#000;
  border-radius:10px;
  position:relative;
}
.video-content iframe{
  width:100%; height:100%;
  border:none;
  border-radius:10px;
}
.close-video{
  position:absolute;
  top:-30px;
  right:0;
  font-size:2rem;
  color:white;
  cursor:pointer;
  transition:0.3s;
}
.close-video:hover{color:#FFD700;}

</style>
</head>
<body>

<header class="header">
  <div class="logo"><i class="fab fa-youtube"></i> ReelTrailers</div>
  <button class="hamburger"><i class="fas fa-bars"></i></button>
  <nav class="menu">
    <ul>
      <li><a href="#home">Home</a></li>
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

<main id="home">
  <section id="acao" class="category-section">
    <div class="category-header"><h2>Ação</h2></div>
    <button class="arrow prev" data-target="acao-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="acao-carousel"></div>
    <button class="arrow next" data-target="acao-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="aventura" class="category-section">
    <div class="category-header"><h2>Aventura</h2></div>
    <button class="arrow prev" data-target="aventura-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="aventura-carousel"></div>
    <button class="arrow next" data-target="aventura-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="romance" class="category-section">
    <div class="category-header"><h2>Romance</h2></div>
    <button class="arrow prev" data-target="romance-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="romance-carousel"></div>
    <button class="arrow next" data-target="romance-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="ficcao" class="category-section">
    <div class="category-header"><h2>Ficção</h2></div>
    <button class="arrow prev" data-target="ficcao-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="ficcao-carousel"></div>
    <button class="arrow next" data-target="ficcao-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="comedia" class="category-section">
    <div class="category-header"><h2>Comédia</h2></div>
    <button class="arrow prev" data-target="comedia-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="comedia-carousel"></div>
    <button class="arrow next" data-target="comedia-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="terror" class="category-section">
    <div class="category-header"><h2>Terror</h2></div>
    <button class="arrow prev" data-target="terror-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="terror-carousel"></div>
    <button class="arrow next" data-target="terror-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>

  <section id="anime" class="category-section">
    <div class="category-header"><h2>Anime</h2></div>
    <button class="arrow prev" data-target="anime-carousel"><i class="fas fa-chevron-left"></i></button>
    <div class="carousel" id="anime-carousel"></div>
    <button class="arrow next" data-target="anime-carousel"><i class="fas fa-chevron-right"></i></button>
  </section>
</main>

<!-- MODAL VIDEO -->
<div class="video-modal" id="video-modal">
  <div class="video-content">
    <span class="close-video">&times;</span>
    <iframe id="video-frame" src="" allow="autoplay; encrypted-media" allowfullscreen></iframe>
  </div>
</div>

<script>
const hamburger=document.querySelector('.hamburger');
const menu=document.querySelector('.menu');
hamburger.addEventListener('click',()=>{menu.classList.toggle('active');});

const API_KEY="23d2fcca011bbb4e5f88ba16f9bede18";
const categories=["acao","aventura","romance","ficcao","comedia","terror","anime"];

function createCard(movie){
  const poster=`https://image.tmdb.org/t/p/w500${movie.poster_path}`;
  return `<div class="card" data-video="https://www.youtube.com/embed/${movie.trailer}">
            <img src="${poster}" alt="">
            <div class="card-overlay"><p>${movie.overview || "Sem sinopse disponível"}</p></div>
          </div>`;
}

async function loadMovies(category, containerId){
  try{
    const response=await fetch(`https://api.themoviedb.org/3/movie/${category}?api_key=${API_KEY}&language=pt-BR`);
    const data=await response.json();
    const container=document.getElementById(containerId);
    container.innerHTML=data.results.map(createCard).join("");
  }catch(e){console.error(e);}
}

// Inicializa categorias
categories.forEach(cat=>{
  loadMovies(cat,`${cat}-carousel`);
});

// CAROUSEL SCROLL
document.querySelectorAll('.arrow').forEach(btn=>{
  btn.addEventListener('click',()=>{
    const container=document.getElementById(btn.dataset.target);
    const scrollAmount=300;
    if(btn.classList.contains('next')) container.scrollBy({left:scrollAmount,behavior:'smooth'});
    else container.scrollBy({left:-scrollAmount,behavior:'smooth'});
  });
});

// VIDEO MODAL
const modal=document.getElementById('video-modal');
const frame=document.getElementById('video-frame');
document.addEventListener('click',e=>{
  if(e.target.closest('.card')){
    const video=e.target.closest('.card').dataset.video;
    frame.src=video+"?autoplay=1";
    modal.style.display="flex";
  }
});
document.querySelector('.close-video').addEventListener('click',()=>{
  modal.style.display="none";
  frame.src="";
});
</script>
</body>
</html>
