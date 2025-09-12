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
        --bg: #121212;
        --text: #fff;
        --gold: #FFD700;
        --card-bg: #1a1a1a;
        --accent: #FF4D4D;
    }
    
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Helvetica Neue', Arial, sans-serif; background: var(--bg); color: var(--text); }
    
    /* Header */
    .header { display: flex; justify-content: space-between; align-items: center; padding: 15px 40px; background: #111; position: sticky; top: 0; z-index: 100; }
    .logo { font-size: 24px; font-weight: bold; color: var(--gold); display: flex; align-items: center; }
    .logo i { margin-right: 5px; }
    .menu ul { display: flex; list-style: none; gap: 20px; }
    .menu a { text-decoration: none; color: white; font-size: 17px; transition: 0.3s; }
    .menu a:hover { color: var(--gold); }
    .hamburger { display: none; font-size: 28px; cursor: pointer; background: none; border: none; color: white; }
    @media (max-width: 768px) {
        .menu { display: none; flex-direction: column; position: absolute; top: 65px; left: 0; width: 100%; background: #111; padding: 20px 0; }
        .menu.active { display: flex; }
        .menu ul { flex-direction: column; gap: 15px; text-align: center; }
        .hamburger { display: block; }
    }
    
    /* Video Carousel */
    .video-carousel-section { 
        position: relative; 
        max-width: 1200px;
        margin: 40px auto; 
        padding: 0 20px;
    }
    .video-carousel { 
        width: 100%; 
        aspect-ratio: 16/9; 
        background: #000; 
        border-radius: 10px;
        overflow: hidden;
    }
    .video-carousel iframe { 
        width: 100%; 
        height: 100%; 
        border: none; 
    }
    .video-carousel-nav { 
        position: absolute; 
        top: 50%; 
        transform: translateY(-50%); 
        background: rgba(0,0,0,0.6); 
        border: none; 
        font-size: 30px; 
        color: var(--gold); 
        cursor: pointer; 
        z-index: 10; 
        padding: 5px 10px; 
        border-radius: 50%; 
        transition: background 0.3s; 
    }
    .video-carousel-nav:hover { 
        background: rgba(0,0,0,0.8); 
    }
    .video-carousel-prev { 
        left: 0; 
    }
    .video-carousel-next { 
        right: 0; 
    }

    @media (max-width: 768px) {
        .video-carousel-section {
            padding: 0;
            margin: 20px 0;
        }
        .video-carousel-nav {
            padding: 2px 5px;
            font-size: 20px;
        }
        .video-carousel-prev {
            left: 10px;
        }
        .video-carousel-next {
            right: 10px;
        }
    }
    
    /* Category Section */
    .category-section { 
        margin: 40px 20px; 
        position: relative;
    }
    .category-header { 
        font-size: 28px; 
        margin-bottom: 15px; 
        font-weight: bold; 
    }
    .card-carousel { 
        display: flex; 
        overflow-x: auto; 
        scroll-behavior: smooth; 
        gap: 15px; 
    }
    .card-carousel::-webkit-scrollbar { 
        display: none; 
    }
    .card { 
        position: relative; 
        width: 200px; 
        height: 300px; 
        flex-shrink: 0; 
        border-radius: 10px; 
        overflow: hidden; 
        cursor: pointer; 
        transition: transform 0.3s, box-shadow 0.3s; 
    }
    .card img { 
        width: 100%; 
        height: 100%; 
        object-fit: cover; 
        display: block; 
    }
    .card:hover { 
        transform: scale(1.05); 
        box-shadow: 0 5px 15px rgba(0,0,0,0.5); 
    }
    
    /* Modal */
    .video-modal { 
        display: none; 
        position: fixed; 
        top: 0; 
        left: 0; 
        width: 100%; 
        height: 100%; 
        background: rgba(20, 20, 20, 0.95); 
        justify-content: center; 
        align-items: center; 
        z-index: 1000; 
    }
    .video-modal-content { 
        position: relative; 
        width: 90%; 
        max-width: 900px; 
        aspect-ratio: 16/9; 
        background: #000; 
        border-radius: 10px; 
        overflow: hidden; 
    }
    .video-modal iframe { 
        width: 100%; 
        height: 100%; 
        border: none; 
    }
    .modal-close-btn { 
        position: absolute; 
        top: -50px; 
        right: 0; 
        color: white; 
        font-size: 2em; 
        cursor: pointer; 
    }
</style>
</head>
<body>

<header class="header">
    <div class="logo"><i class="fab fa-youtube"></i> ReelTrailers</div>
    <button class="hamburger"><i class="fas fa-bars"></i></button>
    <nav class="menu">
        <ul>
            <li><a href="#acao">Ação</a></li>
            <li><a href="#aventura">Aventura</a></li>
            <li><a href="#romance">Romance</a></li>
            <li><a href="#ficcao">Ficção Científica</a></li>
            <li><a href="#comedia">Comédia</a></li>
            <li><a href="#terror">Terror</a></li>
            <li><a href="#anime">Animação</a></li>
        </ul>
    </nav>
</header>

<main>
    <section class="video-carousel-section">
        <button class="video-carousel-nav video-carousel-prev"><i class="fas fa-chevron-left"></i></button>
        <div class="video-carousel" id="main-video-carousel">
            </div>
        <button class="video-carousel-nav video-carousel-next"><i class="fas fa-chevron-right"></i></button>
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
        <h2 class="category-header">Ficção Científica</h2>
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
        <h2 class="category-header">Animação</h2>
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
    const categories = {
        acao: 28,
        aventura: 12,
        romance: 10749,
        ficcao: 878,
        comedia: 35,
        terror: 27,
        anime: 16
    };
    
    const hamburger = document.querySelector('.hamburger');
    const menu = document.querySelector('.menu');
    hamburger.addEventListener('click', () => menu.classList.toggle('active'));
    
    let allMovies = [];
    
    async function getTrailer(id) {
        const res = await fetch(`https://api.themoviedb.org/3/movie/${id}/videos?api_key=${API_KEY}&language=pt-BR`);
        const data = await res.json();
        const trailer = data.results.find(v => v.type === "Trailer" && v.site === "YouTube");
        return trailer ? `https://www.youtube.com/embed/${trailer.key}?autoplay=1&mute=1&controls=0&modestbranding=1&rel=0` : "";
    }
    
    function createCard(movie) {
        const posterUrl = movie.poster_path ? `https://image.tmdb.org/t/p/w500${movie.poster_path}` : 'https://via.placeholder.com/500x750?text=Poster+Not+Found';
        return `<div class="card" data-movie-id="${movie.id}">
            <img src="${posterUrl}" alt="${movie.title}">
        </div>`;
    }
    
    let currentVideoIndex = 0;
    async function initializeVideoCarousel() {
        if (allMovies.length === 0) return;
        const firstMovie = allMovies[0];
        const trailerUrl = await getTrailer(firstMovie.id);
        if (trailerUrl) {
            document.getElementById('main-video-carousel').innerHTML = `<iframe src="${trailerUrl}" allow="autoplay; encrypted-media" allowfullscreen></iframe>`;
        }
    }
    
    function setupVideoCarouselNav() {
        const prevBtn = document.querySelector('.video-carousel-prev');
        const nextBtn = document.querySelector('.video-carousel-next');
    
        prevBtn.addEventListener('click', async () => {
            currentVideoIndex = (currentVideoIndex - 1 + allMovies.length) % allMovies.length;
            const movie = allMovies[currentVideoIndex];
            const trailerUrl = await getTrailer(movie.id);
            if (trailerUrl) {
                document.getElementById('main-video-carousel').innerHTML = `<iframe src="${trailerUrl}" allow="autoplay; encrypted-media" allowfullscreen></iframe>`;
            }
        });
    
        nextBtn.addEventListener('click', async () => {
            currentVideoIndex = (currentVideoIndex + 1) % allMovies.length;
            const movie = allMovies[currentVideoIndex];
            const trailerUrl = await getTrailer(movie.id);
            if (trailerUrl) {
                document.getElementById('main-video-carousel').innerHTML = `<iframe src="${trailerUrl}" allow="autoplay; encrypted-media" allowfullscreen></iframe>`;
            }
        });
    }
    
    async function loadAllMovies() {
        const allMovieData = new Set();
        const uniqueIds = new Set();
    
        for (let cat in categories) {
            let url = `https://api.themoviedb.org/3/discover/movie?api_key=${API_KEY}&with_genres=${categories[cat]}&language=pt-BR`;
            const res = await fetch(url);
            const data = await res.json();
            
            data.results.forEach(movie => {
                if (!uniqueIds.has(movie.id)) {
                    allMovieData.add(movie);
                    uniqueIds.add(movie.id);
                }
            });
        }
    
        allMovies = Array.from(allMovieData);
        populateCategories();
        initializeVideoCarousel();
        setupVideoCarouselNav();
    }
    
    function populateCategories() {
        for (let cat in categories) {
            const container = document.getElementById(`${cat}-carousel`);
            if (container) {
                container.innerHTML = "";
                const moviesForCategory = allMovies.filter(movie => movie.genre_ids.includes(categories[cat]));
                moviesForCategory.forEach(movie => {
                    container.innerHTML += createCard(movie);
                });
                setupCardClickListeners(container);
                setupCarouselButtons(document.getElementById(cat));
            }
        }
    }
    
    function setupCardClickListeners(container) {
        container.querySelectorAll(".card").forEach(card => {
            card.addEventListener("click", async () => {
                const movieId = card.dataset.movieId;
                const trailerUrl = await getTrailer(movieId);
                if (trailerUrl) {
                    openVideo(trailerUrl);
                }
            });
        });
    }
    
    function setupCarouselButtons(section) {
        const container = section.querySelector(".card-carousel");
        const prevBtn = section.querySelector(".prev-button");
        const nextBtn = section.querySelector(".next-button");
        const scrollAmount = 300;
    
        if (prevBtn) {
            prevBtn.addEventListener('click', () => {
                container.scrollLeft -= scrollAmount;
            });
        }
    
        if (nextBtn) {
            nextBtn.addEventListener('click', () => {
                container.scrollLeft += scrollAmount;
            });
        }
    }
    
    const modal = document.getElementById("video-modal");
    const frame = document.getElementById("video-frame");
    document.querySelector(".modal-close-btn").addEventListener("click", () => {
        modal.style.display = "none";
        frame.src = "";
    });
    
    function openVideo(url) {
        modal.style.display = "flex";
        frame.src = url;
    }
    
    loadAllMovies();
</script>
</body>
</html>

