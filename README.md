<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Assista trailers de filmes de ação, aventura, romance, ficção, comédia, terror e anime. Confira os últimos lançamentos no ReelTrailers.">
<meta name="keywords" content="trailers, filmes, lançamentos, cinema, ação, aventura, romance, ficção, comédia, terror, anime">
<meta name="author" content="ReelTrailers">
<meta name="google-adsense-account" content="ca-pub-3305836590830208">
<title>ReelTrailers | Trailers de Filmes e Lançamentos</title>
<link rel="icon" type="image/x-icon" href="http://googleusercontent.com/image_generation_content/0">
<script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=ca-pub-3305836590830208" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

<style>
:root {
    --bg-main: #111;
    --card-bg: #222;
    --text-color-dark: #fff;
    --golden-color: #FFD700;
    --header-bg: #111;
}

body {
    font-family: 'Helvetica Neue', Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: var(--bg-main);
    color: var(--text-color-dark);
    overflow-x: hidden;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 40px;
    background-color: var(--header-bg);
    position: sticky;
    top: 0;
    z-index: 1000;
}

.logo { font-size: 24px; font-weight: bold; color: var(--golden-color); display: flex; align-items: center; }
.logo i { margin-right: 8px; }

.menu ul { list-style: none; display: flex; gap: 20px; margin: 0; padding: 0; }
.menu a { text-decoration: none; color: white; font-weight: 500; transition: color 0.3s; }
.menu a:hover { color: var(--golden-color); }

.hamburger { display: none; font-size: 28px; cursor: pointer; color: white; background: none; border: none; }
.header-icons { display: flex; gap: 25px; font-size: 20px; }
.header-icons i { cursor: pointer; transition: color 0.3s; }
.header-icons i:hover { color: var(--golden-color); }

.content { max-width: 1400px; margin: 20px auto; padding: 0 40px; }
.category-section { margin-bottom: 50px; }
.category-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 15px; }
.category-header h2 { font-size: 28px; color: white; }
.carousel-buttons button { background: transparent; border: none; color: white; font-size: 24px; cursor: pointer; transition: color 0.3s; }
.carousel-buttons button:hover { color: var(--golden-color); }

.card-carousel { display: flex; overflow-x: auto; gap: 20px; scroll-behavior: smooth; }
.card-carousel::-webkit-scrollbar { display: none; }

.card { position: relative; flex-shrink: 0; width: 200px; height: 300px; border-radius: 12px; overflow: hidden; cursor: pointer; transition: transform 0.3s ease, box-shadow 0.3s ease; }
.card img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.3s ease; }
.card:hover { transform: scale(1.05); }

.card-overlay { position: absolute; top:0; left:0; width:100%; height:100%; background: rgba(0,0,0,0.7); color: white; opacity:0; display: flex; flex-direction: column; justify-content: center; align-items: center; padding:10px; text-align:center; transition: opacity 0.3s; }
.card:hover .card-overlay { opacity:1; }
.card-overlay h3 { font-size: 18px; margin-bottom: 8px; }
.card-overlay p { font-size: 14px; }

.video-modal { position: fixed; top:0; left:0; width:100%; height:100%; background: rgba(50,50,50,0.9); display:flex; justify-content:center; align-items:center; z-index:2000; display:none; }
.video-modal-content { position: relative; width:90%; max-width:900px; background:#111; border-radius:10px; box-shadow:0 0 20px #000; overflow:hidden; display:flex; flex-direction:column; }
.video-modal-content iframe { width:100%; height:500px; border:none; border-radius:10px 10px 0 0; }
.modal-close-btn { position:absolute; top:10px; right:15px; font-size:28px; cursor:pointer; color:white; }
.modal-close-btn:hover { color: var(--golden-color); }

@media(max-width:768px){
    .hamburger{display:block;}
    .menu{display:none; position:absolute; top:65px; left:0; width:100%; background:var(--header-bg); flex-direction:column;}
    .menu.active{display:flex;}
    .menu ul{flex-direction:column; gap:15px; text-align:center;}
    .header-icons{display:none;}
    .card{width:150px;height:220px;}
    .category-header h2{font-size:22px;}
}
</style>
</head>
<body>

<header class="header">
    <div class="logo"><i class="fab fa-youtube"></i>ReelTrailers</div>
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
    <div class="header-icons">
        <i class="fas fa-shopping-cart"></i>
        <i class="fas fa-user-circle"></i>
    </div>
</header>

<main class="content" id="home">
    <!-- CATEGORIAS EXISTENTES -->
    <section id="acao" class="category-section">
        <div class="category-header">
            <h2>Ação</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="acao-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="acao-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="acao-carousel"></div>
    </section>

    <section id="aventura" class="category-section">
        <div class="category-header">
            <h2>Aventura</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="aventura-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="aventura-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="aventura-carousel"></div>
    </section>

    <section id="romance" class="category-section">
        <div class="category-header">
            <h2>Romance</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="romance-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="romance-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="romance-carousel"></div>
    </section>

    <!-- NOVAS CATEGORIAS -->
    <section id="ficcao" class="category-section">
        <div class="category-header">
            <h2>Ficção</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="ficcao-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="ficcao-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="ficcao-carousel"></div>
    </section>

    <section id="comedia" class="category-section">
        <div class="category-header">
            <h2>Comédia</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="comedia-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="comedia-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="comedia-carousel"></div>
    </section>

    <section id="terror" class="category-section">
        <div class="category-header">
            <h2>Terror</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="terror-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="terror-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="terror-carousel"></div>
    </section>

    <section id="anime" class="category-section">
        <div class="category-header">
            <h2>Anime</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="anime-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="anime-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="anime-carousel"></div>
    </section>
</main>

<footer class="footer">
    <p>&copy; 2024 ReelTrailers. Todos os direitos reservados.</p>
</footer>

<div class="video-modal" id="video-modal">
    <div class="video-modal-content">
        <i class="fas fa-times modal-close-btn"></i>
        <iframe id="video-frame" src="" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
</div>

<script>
const hamburger = document.querySelector('.hamburger');
const menu = document.querySelector('.menu');
hamburger.addEventListener('click',()=>menu.classList.toggle('active'));

const API_KEY = "23d2fcca011bbb4e5f88ba16f9bede18";

function createCard(movie){
    return `
    <div class="card" onclick="openVideo('${movie.trailer}')">
        <img src="${movie.image}" alt="${movie.title}">
        <div class="card-overlay">
            <h3>${movie.title}</h3>
            <p>${movie.description || "Sem sinopse disponível"}</p>
        </div>
    </div>
    `;
}

const categories = ["acao","aventura","romance","ficcao","comedia","terror","anime"];
categories.forEach(cat=>loadMovies(cat,cat+"-carousel"));

document.querySelectorAll(".next-button, .prev-button").forEach(btn=>{
    btn.addEventListener("click",()=>{
        const containerId = btn.getAttribute("data-container");
        const container = document.getElementById(containerId);
        container.scrollBy({left: btn.classList.contains("next-button")?300:-300, behavior:"smooth"});
    });
});

const modal = document.getElementById("video-modal");
const frame = document.getElementById("video-frame");

function openVideo(url){
    modal.style.display="flex";
    frame.src=url+"?autoplay=1";
}

document.querySelector(".modal-close-btn").addEventListener("click",()=>{
    modal.style.display="none";
    frame.src="";
});

modal.addEventListener("click", (e)=>{
    if(e.target===modal){
        modal.style.display="none";
        frame.src="";
    }
});
</script>

</body>
</html>
