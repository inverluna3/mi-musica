<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carlos Luna Compositor | Sitio Oficial</title>
    <style>
        /* ESTILOS GENERALES (Actualizados: Azul Celeste y Tonos Profundos) */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            background-color: #87CEEB; /* Azul Celeste */
            color: #1a2536; /* Texto oscuro para contraste en fondo claro */
            line-height: 1.6;
        }
        a {
            color: #004080; /* Azul profundo */
            text-decoration: none;
            transition: 0.3s;
            font-weight: bold;
        }
        a:hover {
            color: #00264d;
        }
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
        }

        /* ENCABEZADO */
        header {
            background-color: #004080; /* Azul profundo */
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            border-bottom: 2px solid #00264d;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .logo {
            font-size: 24px;
            font-weight: bold;
            color: #ffffff;
            letter-spacing: 1px;
        }
        .logo span {
            color: #87CEEB; /* Azul celeste en el logo */
        }
        .nav-links {
            list-style: none;
            display: flex;
            gap: 25px;
        }
        .nav-links a { color: #ffffff; }

        /* SECCIÓN HERO (PORTADA) */
        .hero {
            padding: 100px 0;
            text-align: center;
            background: linear-gradient(to bottom, rgba(135,206,235,0.7), #87CEEB);
            border-bottom: 1px solid rgba(0,0,0,0.1);
        }
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #00264d; /* Azul muy profundo */
        }
        .hero h1 span {
            color: #004080; /* Azul profundo */
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 40px auto;
            color: #2c3e50;
        }
        .btn-cta {
            background-color: #004080;
            color: #ffffff;
            padding: 15px 30px;
            font-weight: bold;
            border-radius: 5px;
            font-size: 1.1rem;
            box-shadow: 0 4px 15px rgba(0, 64, 128, 0.3);
        }
        .btn-cta:hover {
            background-color: #00264d;
            color: #ffffff;
            transform: translateY(-2px);
        }

        /* SOBRE MÍ */
        .about {
            padding: 80px 0;
            background-color: rgba(255, 255, 255, 0.4);
        }
        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 50px;
            color: #00264d;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: #004080;
            margin: 10px auto 0 auto;
        }
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }
        @media (max-width: 768px) {
            .about-content { grid-template-columns: 1fr; text-align: center;}
            .nav-links { display: none; }
        }
        .stat-box {
            background-color: #ffffff;
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            flex: 1;
            border: 1px solid #004080;
        }
        .stat-box h3 { font-size: 2rem; color: #004080; }

        /* CATÁLOGO */
        .catalog { padding: 80px 0; }
        .genres-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 25px;
        }
        .genre-card {
            background-color: #ffffff;
            border: 2px solid #004080;
            padding: 30px;
            border-radius: 8px;
            text-align: center;
            transition: 0.3s;
        }
        .genre-card:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.1); }
        .genre-card h3 { color: #004080; margin-bottom: 15px; }
        .video-link {
            display: inline-block;
            margin-top: 15px;
            color: #d32f2f; /* Rojo para destacar el enlace de video */
            text-decoration: underline;
        }

        /* CONTACTO */
        .contact { padding: 80px 0; background-color: rgba(255, 255, 255, 0.4); text-align: center; }
        .contact-info {
            max-width: 600px;
            margin: 0 auto;
            background-color: #ffffff;
            padding: 40px;
            border-radius: 8px;
            border: 2px solid #004080;
        }
        .phone-btn {
            display: inline-block;
            background-color: #25d366;
            color: white !important;
            padding: 12px 25px;
            border-radius: 5px;
            font-weight: bold;
            margin-top: 20px;
        }

        /* FOOTER */
        footer {
            background-color: #004080;
            padding: 30px 0;
            text-align: center;
            font-size: 0.9rem;
            color: #ffffff;
        }
    </style>
</head>
<body>

<header>
    <div class="container nav">
        <div class="logo">Carlos<span>Luna</span></div>
        <ul class="nav-links">
            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#sobre-mi">Biografía</a></li>
            <li><a href="#catalogo">Catálogo</a></li>
            <li><a href="#contacto">Contacto</a></li>
        </ul>
    </div>
</header>

<section id="inicio" class="hero">
    <div class="container">
        <h1>La Letra con Alma, <span>El Sonido del Mañana</span></h1>
        <p>Compositor venezolano fusionando la lírica tradicional con la innovación de la Inteligencia Artificial musical.</p>
        <a href="#catalogo" class="btn-cta">Escuchar Catálogo</a>
    </div>
</section>

<section id="sobre-mi" class="about">
    <div class="container">
        <h2 class="section-title">El Compositor</h2>
        <div class="about-content">
            <div>
                <p>Soy <strong>Carlos Luna</strong>, compositor radicado en Caracas, Venezuela. Mi pasión es dar vida a historias a través de las letras, rompiendo las barreras de los géneros musicales.</p>
            </div>
            <div style="display: flex; gap: 20px;">
                <div class="stat-box">
                    <h3>150+</h3>
                    <p>Temas</p>
                </div>
                <div class="stat-box">
                    <h3>Caracas</h3>
                    <p>Origen</p>
                </div>
            </div>
        </div>
    </div>
</section>

<section id="catalogo" class="catalog">
    <div class="container">
        <h2 class="section-title">Catálogo Musical</h2>
        <div class="genres-grid">
            
            <div class="genre-card">
                <h3>Reggaetón & Urbano</h3>
                <p>Flow moderno y letras comerciales.</p>
                <a href="https://vt.tiktok.com/ZSx8wWuSV/" class="video-link" target="_blank">Seguir este enlace para ver el video</a>
            </div>

            <div class="genre-card">
                <h3>Salsa & Tropical</h3>
                <p>El sabor y la clave del Caribe.</p>
                <a href="https://vt.tiktok.com/ZSx8wyh2b/" class="video-link" target="_blank">Seguir este enlace para ver el video</a>
            </div>

            <div class="genre-card">
                <h3>Baladas</h3>
                <p>Poesía hecha canción.</p>
                <a href="https://vt.tiktok.com/ZSx8wnu6j/" class="video-link" target="_blank">Seguir este enlace para ver el video</a>
            </div>

            <div class="genre-card">
                <h3>Llanera</h3>
                <p>Identidad y sentimiento venezolano.</p>
                <a href="https://vt.tiktok.com/ZSx8wGWyx/" class="video-link" target="_blank">Seguir este enlace para ver el video</a>
            </div>

        </div>
    </div>
</section>

<section id="contacto" class="contact">
    <div class="container">
        <h2 class="section-title">Contacto Profesional</h2>
        <div class="contact-info">
            <p><strong>Ubicación:</strong> Caracas, Venezuela</p>
            <p><strong>TikTok:</strong> @carloslunacompositor.52</p>
            <p><strong>WhatsApp:</strong> 0580416 6069567</p>
            <a href="https://wa.me/584166069567" class="phone-btn" target="_blank">
                Escríbeme por WhatsApp
            </a>
        </div>
    </div>
</section>

<footer>
    <div class="container">
        <p>&copy; 2026 Carlos Luna Compositor | @carloslunacompositor.52</p>
    </div>
</footer>

</body>
</html>
