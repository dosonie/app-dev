# app-dev
My first repository


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sam | Alice in Borderland</title>

    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;600;800&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            background-color: #090909;
            color: white;
            font-family: 'Poppins', sans-serif;
        }

        /* NAVIGATION */
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 25px 8%;
            background: #090909;
        }

        .logo {
            font-family: 'Orbitron', sans-serif;
            color: #e50936;
            font-size: 20px;
            font-weight: 800;
            letter-spacing: 3px;
        }

        nav a {
            color: #ccc;
            text-decoration: none;
            margin-left: 25px;
            font-size: 12px;
            letter-spacing: 1px;
            transition: 0.3s;
        }

        nav a:hover {
            color: #e50936;
        }

        /* HERO */
        .hero {
            height: 85vh;
            display: flex;
            align-items: center;
            padding: 8%;
            background:
                linear-gradient(to right, #090909 15%, rgba(9,9,9,.75), rgba(9,9,9,.25)),
                url('https://images.unsplash.com/photo-1519501025264-65ba15a82390?q=80&w=2000')
                center/cover;
        }

        .hero-content {
            max-width: 650px;
        }

        .hero small {
            color: #e50936;
            letter-spacing: 5px;
            font-size: 11px;
        }

        .hero h1 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(40px, 7vw, 75px);
            line-height: 1.15;
            margin: 20px 0;
        }

        .hero h1 span {
            color: #e50936;
        }

        .hero p {
            color: #bbb;
            line-height: 1.8;
            font-size: 14px;
            max-width: 500px;
        }

        .hero-btn {
            display: inline-block;
            margin-top: 30px;
            padding: 13px 28px;
            background: #e50936;
            color: white;
            text-decoration: none;
            font-size: 11px;
            letter-spacing: 2px;
            transition: .3s;
        }

        .hero-btn:hover {
            background: white;
            color: #e50936;
        }

        /* GENERAL SECTIONS */
        section {
            padding: 90px 10%;
        }

        .section-label {
            color: #e50936;
            font-size: 11px;
            letter-spacing: 4px;
            margin-bottom: 12px;
        }

        .section-title {
            font-family: 'Orbitron', sans-serif;
            font-size: 30px;
            margin-bottom: 25px;
        }

        /* ABOUT */
        .about {
            display: flex;
            align-items: center;
            gap: 60px;
            background: #101010;
        }

        .about-text {
            flex: 1;
        }

        .about-text p {
            color: #aaa;
            font-size: 14px;
            line-height: 2;
        }

        .about-image {
            flex: 1;
        }

        .about-image img {
            width: 100%;
            border-left: 4px solid #e50936;
            display: block;
        }

        /* SERIES */
        .series {
            text-align: center;
        }

        .series-description {
            max-width: 700px;
            margin: 0 auto 45px;
            color: #aaa;
            font-size: 14px;
            line-height: 2;
        }

        .poster-container {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 25px;
        }

        .poster {
            width: 260px;
            background: #151515;
            border-bottom: 3px solid #e50936;
            text-align: left;
            transition: .3s;
        }

        .poster:hover {
            transform: translateY(-8px);
        }

        .poster img {
            width: 100%;
            height: 330px;
            object-fit: cover;
            display: block;
        }

        .poster-info {
            padding: 20px;
        }

        .poster-info h3 {
            font-family: 'Orbitron', sans-serif;
            font-size: 15px;
            margin-bottom: 10px;
        }

        .poster-info p {
            color: #888;
            font-size: 12px;
            line-height: 1.7;
        }

        /* PLAYING CARD SYMBOLS */
        .symbols {
            background: #101010;
            text-align: center;
        }

        .card-symbols {
            display: flex;
            justify-content: center;
            gap: 55px;
            flex-wrap: wrap;
            margin-top: 35px;
        }

        .symbol {
            font-family: 'Orbitron', sans-serif;
            font-size: 55px;
            color: #e50936;
        }

        .symbol p {
            color: #aaa;
            font-family: 'Poppins', sans-serif;
            font-size: 11px;
            letter-spacing: 2px;
            margin-top: 10px;
        }

        /* QUOTE */
        .quote {
            text-align: center;
            padding: 110px 10%;
        }

        .quote h2 {
            font-family: 'Orbitron', sans-serif;
            font-size: clamp(20px, 4vw, 35px);
            line-height: 1.7;
        }

        .quote span {
            color: #e50936;
        }

        /* FOOTER */
        footer {
            background: #050505;
            text-align: center;
            padding: 30px;
            color: #777;
            font-size: 11px;
            letter-spacing: 2px;
            border-top: 1px solid #222;
        }

        /* RESPONSIVE */
        @media (max-width: 768px) {
            nav {
                padding: 20px 5%;
            }

            nav a {
                margin-left: 10px;
                font-size: 10px;
            }

            .hero {
                height: 75vh;
                padding: 7%;
            }

            .about {
                flex-direction: column;
                gap: 30px;
            }

            section {
                padding: 65px 7%;
            }

            .card-symbols {
                gap: 30px;
            }
        }
    </style>
</head>

<body>

    <!-- NAVIGATION -->
    <nav>
        <div class="logo">BORDERLAND.</div>

        <div>
            <a href="#home">HOME</a>
            <a href="#about">ABOUT</a>
            <a href="#series">SERIES</a>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <header class="hero" id="home">
        <div class="hero-content">
            <small>MY FAVORITE SERIES</small>

            <h1>ALICE IN<br><span>BORDERLAND.</span></h1>

            <p>
                A world where survival is the only rule.
                Discover the series that combines mystery,
                strategy, friendship, and psychological thrills.
            </p>

            <a href="#about" class="hero-btn">EXPLORE THE SERIES</a>
        </div>
    </header>

    <!-- ABOUT ME -->
    <section class="about" id="about">

        <div class="about-text">
            <div class="section-label">01 / INTRODUCTION</div>

            <h2 class="section-title">HELLO, I'M SAM.</h2>

            <p>
                Welcome to my website! I'm Sam, and one of my
                favorite television series is Alice in Borderland.
                I enjoy stories that keep me thinking, guessing,
                and excited about what happens next.
                <br><br>
                This website is dedicated to the series,
                its interesting storyline, unforgettable characters,
                and the mysterious world of Borderland.
            </p>
        </div>

        <div class="about-image">
            <img
                src="https://images.unsplash.com/photo-1519608487953-e999c86e7455?q=80&w=1000"
                alt="Tokyo city at night">
        </div>

    </section>

    <!-- SERIES SECTION -->
    <section class="series" id="series">

        <div class="section-label">02 / THE SERIES</div>

        <h2 class="section-title">WELCOME TO BORDERLAND</h2>

        <p class="series-description">
            Alice in Borderland follows Arisu and his friends
            as they find themselves in a mysterious, abandoned
            version of Tokyo. To survive, they must participate
            in dangerous games that test their intelligence,
            physical abilities, and relationships.
        </p>

        <div class="poster-container">

            <div class="poster">
                <img
                    src="https://images.unsplash.com/photo-1519608487953-e999c86e7455?q=80&w=800"
                    alt="Tokyo at night">

                <div class="poster-info">
                    <h3>THE WORLD</h3>
                    <p>
                        An abandoned Tokyo where every day
                        brings a new challenge.
                    </p>
                </div>
            </div>

            <div class="poster">
                <img
                    src="https://images.unsplash.com/photo-1518709268805-4e9042af9f23?q=80&w=800"
                    alt="Mysterious cinematic scenery">

                <div class="poster-info">
                    <h3>THE GAMES</h3>
                    <p>
                        Different challenges that test
                        intelligence, strength, and trust.
                    </p>
                </div>
            </div>

            <div class="poster">
                <img
                    src="https://images.unsplash.com/photo-1511497584788-876760111969?q=80&w=800"
                    alt="Dark forest">

                <div class="poster-info">
                    <h3>THE SURVIVAL</h3>
                    <p>
                        Every decision matters.
                        Every player has a reason to survive.
                    </p>
                </div>
            </div>

        </div>
    </section>

    <!-- CARD SYMBOLS -->
    <section class="symbols">

        <div class="section-label">03 / THE FOUR SUITS</div>

        <h2 class="section-title">KNOW YOUR GAME</h2>

        <div class="card-symbols">

            <div class="symbol">
                ♠
                <p>SPADES</p>
            </div>

            <div class="symbol">
                ♥
                <p>HEARTS</p>
            </div>

            <div class="symbol">
                ♦
                <p>DIAMONDS</p>
            </div>

            <div class="symbol">
                ♣
                <p>CLUBS</p>
            </div>

        </div>

    </section>

    <!-- QUOTE -->
    <section class="quote">

        <div class="section-label">04 / THE BORDERLAND EXPERIENCE</div>

        <h2>
            "IN THIS WORLD,<br>
            <span>SURVIVAL IS EVERYTHING.</span>"
        </h2>

    </section>

    <!-- FOOTER -->
    <footer>
        MADE BY SAM | INSPIRED BY ALICE IN BORDERLAND
    </footer>

</body>
</html>
