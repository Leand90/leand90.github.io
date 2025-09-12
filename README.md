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
            --card-bg: #FFFFFF;
            --text-color-dark: #333;
            --golden-color: #FFD700;
            --green-color: #008000;
            --header-bg: #333;
            --border-color: #555;
        }

        body {
            font-family: 'Helvetica Neue', Arial, sans-serif;
            margin: 0; padding: 0;
            background-color: var(--bg-main);
            color: var(--text-color-dark);
            overflow-x: hidden;
        }

        /* HEADER */
        .header { display: flex; justify-content: space-between; align-items: center; padding: 15px 40px; background-color: var(--header-bg); color: white; position: sticky; top: 0; z-index: 100; }
        .header-left { display: flex; align-items: center; gap: 30px; }
        .logo { font-size: 20px; font-weight: bold; color: var(--golden-color); display: flex; align-items: center; }
        .logo i { font-size: 24px; margin-right: 5px; }
        .menu ul { list-style: none; display: flex; gap: 20px; margin:0; padding:0; }
        .menu a { text-decoration: none; color: white; font-weight: 500; font-size: 17px; transition: color 0.3s; }
        .menu a:hover { color: var(--golden-color); }
        .header-icons { display: flex; gap: 25px; font-size: 20px; }
        .header-icons i { cursor:pointer; transition: color 0.3s; }
        .header-icons i:hover { color: var(--golden-color); }
        .hamburger { display:none; font-size:28px; cursor:pointer; background:none; border:none; color:white; }

        @media(max-width:768px){
            .menu { display:none; flex-direction:column; position:absolute; top:65px; left:0; width:100%; background-color: var(--header-bg); padding:20px 0;}
            .menu.active { display:flex; }
            .menu ul { flex-direction:column; gap:15px; text-align:center;}
            .header-icons { display:none; }
            .hamburger { display:block; }
        }

        /* CATEGORIAS E CARDS */
        .category-section { margin: 50px 20px; color:white; }
        .category-header { display:flex; justify-content:space-between; align-items:center; margin-bottom:20px; }
        .category-header h2 { font-size:28px; border-bottom:3px solid var(--golden-color); display:inline-block; padding-bottom:5px; }
        .carousel-buttons button { background:none; border:none; color:white; font-size:30px; cursor:pointer; transition:color 0.3s; }
        .carousel-buttons button:hover { color:var(--golden-color); }
        .card-carousel { display:flex; overflow-x:auto; scroll-behavior:smooth; gap:20px; -ms-overflow-style:none; scrollbar-width:none; }
        .card-carousel::-webkit-scrollbar { display:none; }

        .card { position:relative; width:200px; height:300px; flex-shrink:0; border-radius:10px; overflow:hidden; cursor:pointer; transition:transform 0.3s; }
        .card img { width:100%; height:100%; object-fit:cover; display:block; }
        .card:hover { transform:translateY(-8px); }

        .card-overlay {
            position:absolute; top:0; left:0; width:100%; height:100%;
            background-color: rgba(0,0,0,0.8); color:white; display:flex; justify-content:center; align-items:center;
            opacity:0; transition:opacity 0.3s; text-align:center; padding:10px; box-sizing:border-box;
        }
        .card:hover .card-overlay { opacity:1; }
        .card-overlay p { font-size:0.9em; line-height:1.2em; }

        /* MODAL DE VIDEO */
        .video-modal { display:none; position:fixed; top:0; left:0; width:100%; height:100%; background-color:rgba(50,50,50,0.8); justify-content:center; align-items:center; z-index:1000; }
        .video-modal-content { position:relative; width:90%; max-width:900px; aspect-ratio:16/9; background-color:#000; border-radius:10px; overflow:hidden; }
        .video-modal-content iframe { width:100%; height:100%; border:none; }
        .modal-close-btn { position:absolute; top:-40px; right:0; color:white; font-size:2em; cursor:pointer; }

    </style>
</head>
<body>

    <header class="header">
        <div class="header-left">
            <div class="logo"><i class="fab fa-youtube"></i> ReelTrailers</div>
        </div>
        <button class="hamburger"><i class="fas fa-bars"></i></button>
        <nav class="menu"><ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#acao">Ação</a></li>
            <li><a href="#aventura">Aventura</a></li>
            <li><a href="#romance">Romance</a></li>
            <li><a href="#ficcao">Ficção</a></li>
            <li><a href="#comedia">Comédia</a></li>
            <li><a href="#terror">Terror</a></li>
            <li><a href="#anime">Anime</a></li>
        </ul></nav>
        <div class="header-icons">
            <i class="fas fa-shopping-cart"></i>
            <i class="fas fa-user-circle"></i>
        </div>
    </header>

    <main id="home"></main>

    <!-- Categorias -->
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

    <!-- MODAL -->
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
        hamburger.addEventListener('click', ()=> menu.classList.toggle('active'));

        function createCard(movie, trailerUrl){
            return `<div class="card" onclick="openVideo('${trailerUrl}')">
                <img src="https://image.tmdb.org/t/p/w500${movie.poster_path}" alt="${movie.title}">
                <div class="card-overlay"><p>${movie.overview}</p></div>
            </div>`;
        }

        async function getTrailer(movie_id){
            const res = await fetch(`https://api.themoviedb.org/3/movie/${movie_id}/videos?api_key=${API_KEY}&language=pt-BR`);
            const data = await res.json();
            const trailer = data.results.find(v => v.type === "Trailer" && v.site==="YouTube");
            return trailer ? `https://www.youtube.com/embed/${trailer.key}?autoplay=1` : "";
        }

        async function loadCategory(categoryName, containerId){
            const genreId = categories[categoryName];
            const res = await fetch(`https://api.themoviedb.org/3/discover/movie?api_key=${API_KEY}&with_genres=${genreId}&language=pt-BR`);
            const data = await res.json();
            const container = document.getElementById(containerId);
            container.innerHTML = "";
            for(let movie of data.results){
                const trailerUrl = await getTrailer(movie.id);
                if(trailerUrl) container.innerHTML += createCard(movie, trailerUrl);
            }
        }

        document.querySelectorAll(".next-button").forEach(btn=>{
            btn.addEventListener('click', ()=>{
                const container = document.getElementById(btn.dataset.container);
                container.scrollBy({left:300, behavior:'smooth'});
            });
        });
        document.querySelectorAll(".prev-button").forEach(btn=>{
            btn.addEventListener('click', ()=>{
                const container = document.getElementById(btn.dataset.container);
                container.scrollBy({left:-300, behavior:'smooth'});
            });
        });

        async function loadAllCategories(){
            for(let cat in categories){
                await loadCategory(cat, `${cat}-carousel`);
            }
        }
        loadAllCategories();

        const modal = document.getElementById("video-modal");
        const frame = document.getElementById("video-frame");
        document.querySelector(".modal-close-btn").addEventListener("click", ()=> { modal.style.display="none"; frame.src=""; });
        function openVideo(url){ modal.style.display="flex"; frame.src=url; }
    </script>
</body>
</html>
