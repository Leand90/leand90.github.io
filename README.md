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
:root {
    --bg-main: #800020;
    --card-bg: #111;
    --text-color-dark: #fff;
    --golden-color: #FFD700;
    --header-bg: #222;
    --border-color: #555;
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
    z-index: 100;
}

.header-left {
    display: flex;
    align-items: center;
    gap: 30px;
}

.logo {
    font-size: 20px;
    font-weight: bold;
    color: var(--golden-color);
    display: flex;
    align-items: center;
}

.logo i {
    font-size: 24px;
    margin-right: 5px;
}

.menu {
    display: flex;
}

.menu ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    gap: 20px;
}

.menu a {
    text-decoration: none;
    color: white;
    font-weight: 500;
    font-size: 17px;
    transition: color 0.3s;
}

.menu a:hover {
    color: var(--golden-color);
}

.hamburger {
    display: none;
    font-size: 28px;
    cursor: pointer;
    color: white;
    background: none;
    border: none;
}

/* Mobile */
@media (max-width: 768px) {
    .menu {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 65px;
        left: 0;
        width: 100%;
        background-color: var(--header-bg);
        padding: 20px 0;
    }
    .menu.active { display: flex; }
    .menu ul { flex-direction: column; gap: 15px; text-align: center; }
    .hamburger { display: block; }
}

/* Carousel */
.category-section {
    margin: 40px 0;
    padding: 0 40px;
}

.category-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}

.category-header h2 { color: white; }

.card-carousel {
    display: flex;
    gap: 15px;
    overflow-x: auto;
    scroll-behavior: smooth;
}

.card-carousel::-webkit-scrollbar { display: none; }

.card {
    position: relative;
    width: 200px;
    height: 300px;
    background-color: var(--card-bg);
    border-radius: 10px;
    overflow: hidden;
    cursor: pointer;
    flex-shrink: 0;
}

.card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.card-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.7);
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    opacity: 0;
    padding: 10px;
    transition: opacity 0.3s ease;
}

.card:hover .card-overlay { opacity: 1; }

.card-overlay h3 {
    font-size: 16px;
    color: var(--golden-color);
    margin-bottom: 5px;
}

.card-overlay p { font-size: 14px; }

/* Modal */
.video-modal {
    display: none;
    position: fixed;
    top:0; left:0;
    width:100%;
    height:100%;
    background-color: rgba(0,0,0,0.8);
    justify-content: center;
    align-items: center;
    z-index: 999;
}

.video-modal-content {
    position: relative;
    width: 90%;
    max-width: 900px;
    background-color: #000;
    border-radius: 10px;
}

.modal-close-btn {
    position: absolute;
    top: -30px;
    right: 0;
    color: white;
    font-size: 2em;
    cursor: pointer;
}

.modal-close-btn:hover { color: var(--golden-color); }

.carousel-buttons { display: flex; gap: 10px; }

.carousel-buttons button {
    background: rgba(0,0,0,0.5);
    border: none;
    color: white;
    font-size: 24px;
    cursor: pointer;
    border-radius: 50%;
    padding: 5px 10px;
}

.carousel-buttons button:hover { background: var(--golden-color); }

</style>
</head>
<body>

<header class="header">
    <div class="header-left">
        <div class="logo"><i class="fab fa-youtube"></i> ReelTrailers</div>
    </div>

    <button class="hamburger" aria-label="Abrir menu"><i class="fas fa-bars"></i></button>

    <nav class="menu">
        <ul>
            <li><a href="#lancamentos">Home</a></li>
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
        <div class="category-header">
            <h2>Lançamentos</h2>
            <div class="carousel-buttons">
                <button class="prev-button" data-container="lancamentos-carousel"><i class="fas fa-chevron-left"></i></button>
                <button class="next-button" data-container="lancamentos-carousel"><i class="fas fa-chevron-right"></i></button>
            </div>
        </div>
        <div class="card-carousel" id="lancamentos-carousel"></div>
    </section>

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

<div class="video-modal" id="video-modal">
    <div class="video-modal-content">
        <span class="modal-close-btn" id="modal-close">&times;</span>
        <iframe id="video-frame" width="100%" height="500" frameborder="0" allowfullscreen></iframe>
    </div>
</div>

<script>
const hamburger = document.querySelector('.hamburger');
const menu = document.querySelector('.menu');
hamburger.addEventListener('click', () => { menu.classList.toggle('active'); });

const API_KEY = '23d2fcca011bbb4e5f88ba16f9bede18';
const BASE_URL = 'https://api.themoviedb.org/3';

const categories = {
    lancamentos: '/movie/now_playing',
    acao: '/discover/movie?with_genres=28',
    aventura: '/discover/movie?with_genres=12',
    romance: '/discover/movie?with_genres=10749',
    ficcao: '/discover/movie?with_genres=878',
    comedia: '/discover/movie?with_genres=35',
    terror: '/discover/movie?with_genres=27',
    anime: '/discover/movie?with_genres=16'
};

function createCard(movie) {
    const poster = `https://image.tmdb.org/t/p/w500${movie.poster_path}`;
    return `
        <div class="card" data-video="${movie.id}">
            <img src="${poster}" alt="${movie.title}">
            <div class="card-overlay">
                <h3>${movie.title}</h3>
                <p>${movie.overview || "Sem sinopse disponível"}</p>
            </div>
        </div>
    `;
}

async function loadMovies(categoryKey, containerId) {
    try {
        const response = await fetch(`${BASE_URL}${categories[categoryKey]}&api_key=${API_KEY}&language=pt-BR&page=1`);
        const data = await response.json();
        const container = document.getElementById(containerId);
        container.innerHTML = data.results.map(createCard).join('');
    } catch (e) { console.error(e); }
}

// Carousel scroll
document.addEventListener('click', e => {
    if(e.target.closest('.next-button')) {
        const containerId = e.target.closest('button').dataset.container;
        document.getElementById(containerId).scrollBy({ left: 300, behavior: 'smooth' });
    }
    if(e.target.closest('.prev-button')) {
        const containerId = e.target.closest('button').dataset.container;
        document.getElementById(containerId).scrollBy({ left: -300, behavior: 'smooth' });
    }
});

// Modal
const modal = document.getElementById('video-modal');
const modalClose = document.getElementById('modal-close');
const videoFrame = document.getElementById('video-frame');

document.addEventListener('click', async e => {
    const card = e.target.closest('.card');
    if(card) {
        const movieId = card.dataset.video;
        try {
            const response = await fetch(`${BASE_URL}/movie/${movieId}/videos?api_key=${API_KEY}&language=pt-BR`);
            const data = await response.json();
            const trailer = data.results.find(v => v.type==='Trailer' && v.site==='YouTube');
            if(trailer) {
                videoFrame.src = `https://www.youtube.com/embed/${trailer.key}?autoplay=1&rel=0`;
                modal.style.display = 'flex';
            }
        } catch(e){ console.error(e); }
    }
});

modalClose.addEventListener('click', () => {
    videoFrame.src = '';
    modal.style.display = 'none';
});

// Inicializar
for(const cat in categories) loadMovies(cat, `${cat}-carousel`);
</script>
</body>
</html>
