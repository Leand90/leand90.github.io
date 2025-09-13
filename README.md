<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Assista trailers de filmes de ação, aventura, romance, drama, suspense e terror. Confira os últimos lançamentos no Trai-llers.">
<meta name="keywords" content="trailers, filmes, lançamentos, cinema, ação, aventura, romance, drama, suspense, terror">
<meta name="author" content="Leandro Santana">
<meta name="google-site-verification" content="b7F2kMlRsWM-RXTOU7jN6dnEDPGR91Q8dI3AnyUy6G8" />
<meta name="google-adsense-account" content="ca-pub-3305836590830208">
<title>Trai-llers | Trailers de Filmes e Lançamentos</title>
<link rel="icon" type="image/x-icon" href="http://googleusercontent.com/image_generation_content/0">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
<script data-ad-client="pub-3305836590830208" async
    src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js?client=pub-3305836590830208"
    crossorigin="anonymous"></script>
<link rel="stylesheet" href="style.css">
</head>
<body>

<!-- HEADER -->
<header class="header">
    <div class="logo"><i class="fas fa-film"></i> Trai-llers</div>
    <button class="hamburger"><i class="fas fa-bars"></i></button>
    <nav class="menu">
        <ul>
            <li><a href="#lancamentos">Lançamentos</a></li>
            <li><a href="#acao">Ação</a></li>
            <li><a href="#aventura">Aventura</a></li>
            <li><a href="#romance">Romance</a></li>
            <li><a href="#ficcao">Ficcao Cientifica</a></li>
            <li><a href="#comedia">Comedia</a></li>
            <li><a href="#terror">Terror</a></li>
            <li><a href="#anime">Animacão</a></li>
            <li><a href="#series">Series</a></li>
        </ul>
    </nav>
</header>

<!-- MAIN -->
<main>
    <!-- CATEGORIAS -->
    <section id="lancamentos" class="category-section">
        <h2 class="category-header">Lançamentos</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="lancamentos-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="acao" class="category-section">
        <h2 class="category-header">Ação</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="acao-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="aventura" class="category-section">
        <h2 class="category-header">Aventura</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="aventura-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="romance" class="category-section">
        <h2 class="category-header">Romance</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="romance-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="ficcao" class="category-section">
        <h2 class="category-header">Ficção Cientifica</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="ficcao-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="comedia" class="category-section">
        <h2 class="category-header">Comédia</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="comedia-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="terror" class="category-section">
        <h2 class="category-header">Terror</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="terror-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="anime" class="category-section">
        <h2 class="category-header">Animação</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="anime-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

    <section id="series" class="category-section">
        <h2 class="category-header">Series Populares</h2>
        <div class="card-carousel-container">
            <button class="carousel-button prev-button"><i class="fas fa-chevron-left"></i></button>
            <div class="card-carousel" id="series-carousel"></div>
            <button class="carousel-button next-button"><i class="fas fa-chevron-right"></i></button>
        </div>
    </section>

</main>

<!-- MODAL VIDEO -->
<div class="video-modal" id="video-modal">
    <div class="video-modal-content">
        <i class="fas fa-times modal-close-btn"></i>
        <iframe id="video-frame" src="" allow="autoplay; encrypted-media" allowfullscreen></iframe>
    </div>
</div>

<!-- FOOTER -->
<footer class="footer">
    <div class="footer-content" style="display:flex; justify-content:center; gap:10px; flex-wrap:wrap; font-size:14px;">
        <span>Criado com ❤️ por Leandro Santana</span>
        <span>|</span>
        <span>Contato: <a href="mailto:ldsantana692@gmail.com">ldsantana692@gmail.com</a></span>
        <span>|</span>
        <span>© 2025 Trai-llers — Todos os direitos reservados.</span>
    </div>
</footer>

<!-- JAVASCRIPT -->
<script>
const API_KEY = "23d2fcca011bbb4e5f88ba16f9bede18";

// MENU RESPONSIVO
const hamburger = document.querySelector('.hamburger');
const menu = document.querySelector('.menu');
hamburger.addEventListener('click', () => menu.classList.toggle('active'));

document.querySelectorAll('.menu a').forEach(link => {
    link.addEventListener('click', e => {
        e.preventDefault();
        const target = document.querySelector(link.getAttribute('href'));
        if(target) target.scrollIntoView({ behavior: 'smooth', block: 'start' });
        menu.classList.remove('active');
    });
});

// CATEGORIAS
const categories = {
    lancamentos: '',
    acao: 28,
    aventura: 12,
    romance: 10749,
    ficcao: 878,
    comedia: 35,
    terror: 27,
    anime: 16,
    series: "tv"
};

// FUNÇÃO TRAILER
async function getTrailer(id, type="movie") {
    const res = await fetch(`https://api.themoviedb.org/3/${type}/${id}/videos?api_key=${API_KEY}&language=pt-BR`);
    const data = await res.json();
    const trailer = data.results.find(v => v.type === "Trailer" && v.site === "YouTube");
    return trailer ? `https://www.youtube.com/embed/${trailer.key}?autoplay=1&controls=0&modestbranding=1&rel=0` : "";
}

// CRIAR CARD
function createCard(item, type="movie") {
    const posterUrl = item.poster_path ? `https://image.tmdb.org/t/p/w500${item.poster_path}` : 'https://via.placeholder.com/500x750?text=Poster+Not+Found';
    const overview = item.overview ? item.overview.slice(0, 120) + "..." : "Sem sinopse";
    const title = type === "tv" ? item.name : item.title;
    return `<div class="card" data-id="${item.id}" data-type="${type}">
        <img src="${posterUrl}" alt="${title}">
        <div class="card-overlay">${overview}</div>
    </div>`;
}

// CARREGAR CATEGORIAS
async function loadAllCategories() {
    const fetchPromises = [];
    for(const cat in categories){
        let url, type="movie";
        if(cat === "lancamentos"){
            url = `https://api.themoviedb.org/3/movie/now_playing?api_key=${API_KEY}&language=pt-BR`;
        } else if(cat === "series"){
            url = `https://api.themoviedb.org/3/tv/popular?api_key=${API_KEY}&language=pt-BR`;
            type="tv";
        } else {
            url = `https://api.themoviedb.org/3/discover/movie?api_key=${API_KEY}&with_genres=${categories[cat]}&language=pt-BR`;
        }
        fetchPromises.push(fetch(url).then(res => res.json()).then(data => ({category:cat, items:data.results, type})));
    }
    try {
        const results = await Promise.all(fetchPromises);
        results.forEach(result => {
            const container = document.getElementById(`${result.category}-carousel`);
            if(container){
                container.innerHTML = "";
                result.items.forEach(item => container.innerHTML += createCard(item, result.type));
                setupCardClickListeners(container);
                setupCarouselButtons(container.parentElement);
            }
        });
    } catch(err){
        console.error("Erro ao carregar categorias:", err);
    }
}

// CARDS CLICK
function setupCardClickListeners(container){
    container.querySelectorAll(".card").forEach(card=>{
        card.addEventListener("click", async ()=>{
            const trailerUrl = await getTrailer(card.dataset.id, card.dataset.type);
            if(trailerUrl) openVideo(trailerUrl);
        });
    });
}

// CARROSSEL
function setupCarouselButtons(section){
    const container = section.querySelector(".card-carousel");
    const prevBtn = section.querySelector(".prev-button");
    const nextBtn = section.querySelector(".next-button");
    const scrollAmount = 300;
    if(prevBtn && nextBtn){
        prevBtn.addEventListener('click', ()=>container.scrollLeft -= scrollAmount);
        nextBtn.addEventListener('click', ()=>container.scrollLeft += scrollAmount);
    }
}

// MODAL VIDEO
const modal = document.getElementById("video-modal");
const frame = document.getElementById("video-frame");
function openVideo(url){
    modal.style.display = "flex";
    frame.src = url;
}
document.querySelector(".modal-close-btn").addEventListener('click', ()=>{
    modal.style.display = "none";
    frame.src = "";
});

// INICIAR
loadAllCategories();
</script>

</body>
</html>
