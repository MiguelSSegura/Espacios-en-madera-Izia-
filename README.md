<!DOCTYPE html>
<html lang="es-MX">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>IZIA | Espacios en Madera | Cocinas y Diseño Residencial</title>

    <meta name="description"
        content="IZIA, Espacios en Madera. Diseño y fabricación de cocinas, muebles y espacios residenciales combinando madera, piedra, granito y cuarzo. Atención en el sur de Tamaulipas, norte de Veracruz y Huasteca Potosina.">

    <meta name="keywords"
        content="cocinas en Tampico, cocinas integrales Tampico, diseño de cocinas, cocinas de madera, cocinas con granito, cocinas con cuarzo, diseño residencial Tampico, muebles de madera, cocinas Madero, cocinas Altamira, cocinas norte de Veracruz, cocinas Huasteca Potosina">

    <meta name="author" content="IZIA, Espacios en Madera">

    <meta property="og:title"
        content="IZIA | Espacios en Madera">
    <meta property="og:description"
        content="Diseñamos cocinas y espacios residenciales combinando la calidez de la madera con la elegancia de la piedra.">
    <meta property="og:type" content="website">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Montserrat:wght@300;400;500;600;700&display=swap"
        rel="stylesheet">

    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>

        :root {
            --madera: #6f4a32;
            --madera-oscura: #33241b;
            --carbon: #171717;
            --piedra: #d8d1c5;
            --arena: #eee9e1;
            --blanco: #ffffff;
            --dorado: #b89a68;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background: var(--blanco);
            color: var(--carbon);
            line-height: 1.6;
        }

        img {
            max-width: 100%;
            display: block;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* =========================
           HEADER
        ========================== */

        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background: rgba(23,23,23,.92);
            backdrop-filter: blur(12px);
        }

        .nav {
            max-width: 1250px;
            margin: auto;
            height: 78px;
            padding: 0 25px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            color: white;
            font-family: 'Cormorant Garamond', serif;
            font-size: 31px;
            font-weight: 600;
            letter-spacing: 2px;
        }

        .logo span {
            display: block;
            font-family: 'Montserrat', sans-serif;
            font-size: 9px;
            letter-spacing: 4px;
            color: var(--dorado);
            margin-top: -5px;
        }

        .menu {
            display: flex;
            gap: 28px;
            list-style: none;
        }

        .menu a {
            color: white;
            font-size: 13px;
            transition: .3s;
        }

        .menu a:hover {
            color: var(--dorado);
        }

        .menu-btn {
            display: none;
            color: white;
            font-size: 28px;
            cursor: pointer;
        }

        /* =========================
           HERO
        ========================== */

        .hero {
            min-height: 100vh;
            background:
                linear-gradient(rgba(20,15,12,.48), rgba(20,15,12,.70)),
                url("https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=2000&q=85")
                center/cover;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            padding: 120px 20px 70px;
        }

        .hero-content {
            max-width: 850px;
        }

        .hero small {
            text-transform: uppercase;
            letter-spacing: 5px;
            color: #e5d2ae;
            font-size: 12px;
        }

        .hero h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: clamp(55px, 8vw, 105px);
            line-height: .9;
            margin: 20px 0;
        }

        .hero h2 {
            font-weight: 300;
            font-size: clamp(18px, 3vw, 28px);
            margin-bottom: 25px;
        }

        .hero p {
            max-width: 650px;
            margin: auto;
            color: #eee;
        }

        .buttons {
            margin-top: 35px;
            display: flex;
            justify-content: center;
            gap: 14px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 14px 26px;
            border: 1px solid white;
            color: white;
            font-size: 12px;
            letter-spacing: 1px;
            transition: .3s;
        }

        .btn.primary {
            background: var(--madera);
            border-color: var(--madera);
        }

        .btn:hover {
            transform: translateY(-3px);
            background: var(--dorado);
            border-color: var(--dorado);
        }

        /* =========================
           GENERAL
        ========================== */

        section {
            padding: 100px 20px;
        }

        .container {
            max-width: 1200px;
            margin: auto;
        }

        .section-title {
            text-align: center;
            max-width: 700px;
            margin: 0 auto 55px;
        }

        .section-title small {
            color: var(--madera);
            letter-spacing: 3px;
            text-transform: uppercase;
            font-size: 11px;
        }

        .section-title h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: clamp(40px, 6vw, 65px);
            line-height: 1;
            margin: 12px 0;
        }

        .section-title p {
            color: #666;
        }

        /* =========================
           INTRO
        ========================== */

        .intro {
            background: var(--arena);
        }

        .intro-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
            align-items: center;
        }

        .intro-image {
            height: 600px;
            background:
                url("https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?auto=format&fit=crop&w=1200&q=85")
                center/cover;
        }

        .intro-text h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 55px;
            line-height: 1;
            margin-bottom: 25px;
        }

        .intro-text p {
            margin-bottom: 20px;
            color: #555;
        }

        /* =========================
           CATEGORIAS
        ========================== */

        .cards {
            display: grid;
            grid-template-columns: repeat(3,1fr);
            gap: 20px;
        }

        .card {
            min-height: 450px;
            position: relative;
            overflow: hidden;
            color: white;
        }

        .card img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            position: absolute;
            transition: transform .7s;
        }

        .card:hover img {
            transform: scale(1.06);
        }

        .card-overlay {
            position: absolute;
            inset: 0;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;
            padding: 35px;
            background: linear-gradient(transparent, rgba(0,0,0,.78));
        }

        .card h3 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 38px;
        }

        .card p {
            font-size: 13px;
            color: #eee;
        }

        /* =========================
           COMBINACIONES
        ========================== */

        .combinations {
            background: var(--carbon);
            color: white;
        }

        .combination-grid {
            display: grid;
            grid-template-columns: repeat(4,1fr);
            gap: 15px;
        }

        .material {
            height: 300px;
            position: relative;
            overflow: hidden;
        }

        .material img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: .5s;
        }

        .material:hover img {
            transform: scale(1.07);
        }

        .material span {
            position: absolute;
            bottom: 20px;
            left: 20px;
            font-size: 13px;
            letter-spacing: 1px;
            background: rgba(0,0,0,.6);
            padding: 8px 13px;
        }

        /* =========================
           PROYECTOS
        ========================== */

        .projects {
            display: grid;
            grid-template-columns: 2fr 1fr 1fr;
            grid-auto-rows: 250px;
            gap: 15px;
        }

        .project {
            overflow: hidden;
        }

        .project:first-child {
            grid-row: span 2;
        }

        .project img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: .5s;
        }

        .project:hover img {
            transform: scale(1.05);
        }

        /* =========================
           ZONAS
        ========================== */

        .zones {
            background: var(--arena);
        }

        .zones-grid {
            display: grid;
            grid-template-columns: repeat(3,1fr);
            gap: 20px;
        }

        .zone {
            background: white;
            padding: 35px;
            text-align: center;
            border-top: 3px solid var(--madera);
        }

        .zone h3 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 32px;
            margin-bottom: 15px;
        }

        .zone p {
            color: #666;
            font-size: 14px;
        }

        /* =========================
           CTA
        ========================== */

        .cta {
            background:
                linear-gradient(rgba(35,25,18,.75),rgba(35,25,18,.75)),
                url("https://images.unsplash.com/photo-1600607687920-4e2a09cf159d?auto=format&fit=crop&w=2000&q=85")
                center/cover;
            color: white;
            text-align: center;
        }

        .cta h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: clamp(45px,6vw,75px);
            line-height: 1;
            margin-bottom: 20px;
        }

        .cta p {
            max-width: 600px;
            margin: auto;
            color: #eee;
        }

        /* =========================
           CONTACTO
        ========================== */

        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 60px;
        }

        .contact-info h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 55px;
            line-height: 1;
            margin-bottom: 20px;
        }

        .contact-info p {
            color: #666;
            margin-bottom: 20px;
        }

        form {
            display: grid;
            gap: 15px;
        }

        input,
        textarea {
            width: 100%;
            padding: 16px;
            border: 1px solid #ddd;
            font-family: inherit;
            outline: none;
        }

        textarea {
            height: 150px;
            resize: vertical;
        }

        form button {
            padding: 16px;
            border: none;
            background: var(--madera);
            color: white;
            cursor: pointer;
            font-weight: 600;
            letter-spacing: 1px;
            transition: background .3s;
        }

        form button:hover {
            background: var(--dorado);
        }

        /* =========================
           FOOTER
        ========================== */

        footer {
            background: #111;
            color: white;
            text-align: center;
            padding: 45px 20px;
        }

        footer h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 40px;
        }

        footer p {
            color: #aaa;
            font-size: 12px;
            margin-top: 10px;
        }

        /* =========================
           CONTACTO FLOTANTE
        ========================== */

        .floating {
            position: fixed;
            right: 18px;
            bottom: 20px;
            z-index: 2000;
        }

        .float-main {
            width: 58px;
            height: 58px;
            border-radius: 50%;
            background: var(--madera);
            color: white;
            border: none;
            cursor: pointer;
            font-size: 25px;
            box-shadow: 0 5px 20px rgba(0,0,0,.25);
            transition: transform .3s, background .3s;
        }

        .floating.active .float-main {
            transform: rotate(45deg);
            background: var(--dorado);
        }

        .float-menu {
            position: absolute;
            right: 0;
            bottom: 70px;
            display: flex;
            flex-direction: column;
            gap: 10px;
            opacity: 0;
            pointer-events: none;
            transform: translateY(15px);
            transition: .3s;
        }

        .floating.active .float-menu {
            opacity: 1;
            pointer-events: auto;
            transform: translateY(0);
        }

        .float-item {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,.2);
            transition: transform .2s;
        }

        .float-item:hover {
            transform: scale(1.1);
        }

        .whatsapp {
            background: #25D366;
        }

        .facebook {
            background: #1877F2;
        }

        .email {
            background: #555;
        }

        /* =========================
           RESPONSIVE
        ========================== */

        @media(max-width: 900px) {

            .menu {
                position: absolute;
                top: 78px;
                left: 0;
                width: 100%;
                background: #171717;
                flex-direction: column;
                align-items: center;
                padding: 25px;
                display: none;
            }

            .menu.active {
                display: flex;
            }

            .menu-btn {
                display: block;
            }

            .intro-grid,
            .contact-grid {
                grid-template-columns: 1fr;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            .combination-grid {
                grid-template-columns: repeat(2,1fr);
            }

            .zones-grid {
                grid-template-columns: 1fr;
            }

            .intro-image {
                height: 450px;
            }
        }

        @media(max-width: 600px) {

            section {
                padding: 70px 18px;
            }

            .nav {
                height: 68px;
            }

            .logo {
                font-size: 25px;
            }

            .hero {
                min-height: 90vh;
            }

            .hero h1 {
                font-size: 62px;
            }

            .hero h2 {
                font-size: 20px;
            }

            .buttons {
                flex-direction: column;
            }

            .btn {
                width: 100%;
            }

            .intro-text h2,
            .contact-info h2 {
                font-size: 45px;
            }

            .combination-grid {
                grid-template-columns: 1fr 1fr;
            }

            .material {
                height: 220px;
            }

            .projects {
                display: grid;
                grid-template-columns: 1fr;
                grid-auto-rows: 230px;
            }

            .project:first-child {
                grid-row: auto;
            }

            .float-main {
                width: 55px;
                height: 55px;
            }

            .float-item {
                width: 46px;
                height: 46px;
            }
        }

    </style>
</head>

<body>

<header>

    <nav class="nav">

        <a href="#inicio" class="logo">
            IZIA
            <span>ESPACIOS EN MADERA</span>
        </a>

        <div class="menu-btn" onclick="toggleMenu()">☰</div>

        <ul class="menu" id="menu">

            <li><a href="#inicio">Inicio</a></li>
            <li><a href="#nosotros">Nosotros</a></li>
            <li><a href="#especialidades">Especialidades</a></li>
            <li><a href="#materiales">Materiales</a></li>
            <li><a href="#proyectos">Proyectos</a></li>
            <li><a href="#contacto">Contacto</a></li>

        </ul>

    </nav>

</header>


<!-- HERO -->

<section class="hero" id="inicio">

    <div class="hero-content">

        <small>Diseño · Madera · Piedra</small>

        <h1>IZIA</h1>

        <h2>Espacios en Madera</h2>

        <p>
            Diseñamos cocinas y espacios residenciales a medida,
            combinando la calidez de la madera con la elegancia
            y personalidad de la piedra.
        </p>

        <div class="buttons">

            <a class="btn primary" href="#proyectos">
                VER PROYECTOS
            </a>

            <!-- SUSTITUIR 'TUNUMERO' POR TU NÚMERO DE WHATSAPP REAL (Ej: 528331234567) -->
            <a class="btn" href="https://wa.me/TUNUMERO" target="_blank" rel="noopener">
                COTIZAR POR WHATSAPP
            </a>

        </div>

    </div>

</section>


<!-- NOSOTROS -->

<section id="nosotros">

    <div class="container intro-grid">

        <div class="intro-image"></div>

        <div class="intro-text">

            <small>IZIA · Diseño residencial</small>

            <h2>Donde la madera encuentra a la piedra.</h2>

            <p>
                Creamos espacios que combinan materiales,
                texturas y proporciones para conseguir
                ambientes únicos y atemporales.
            </p>

            <p>
                Nuestro enfoque integra diseño, fabricación
                y selección de materiales para desarrollar
                proyectos residenciales personalizados.
            </p>

            <a class="btn"
               style="display:inline-block;background:#6f4a32;border-color:#6f4a32;"
               href="#contacto">
                HABLAR CON IZIA
            </a>

        </div>

    </div>

</section>


<!-- ESPECIALIDADES -->
<section id="especialidades">

    <div class="container">

        <div class="section-title">

            <small>Nuestras especialidades</small>

            <h2>Diseñamos espacios para vivirlos.</h2>

            <p>
                Cada proyecto comienza con una idea y termina
                en un espacio diseñado alrededor de quien lo habita.
            </p>

        </div>


        <div class="cards">

            <div class="card">

                <img src="https://images.unsplash.com/photo-1600566753086-00f18fb6b3ea?auto=format&fit=crop&w=1000&q=85" alt="Cocina residencial personalizada">

                <div class="card-overlay">

                    <h3>Cocinas</h3>

                    <p>
                        Diseño y fabricación de cocinas
                        residenciales personalizadas.
                    </p>

                </div>

            </div>

            <div class="card">

                <img src="https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?auto=format&fit=crop&w=1000&q=85" alt="Muebles de madera y carpintería arquitectónica">

                <div class="card-overlay">

                    <h3>Muebles & Carpintería</h3>

                    <p>
                        Mobiliario a medida, vestidores, clósets
                        y detalles arquitectónicos en madera.
                    </p>

                </div>

            </div>

            <div class="card">

                <img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c?auto=format&fit=crop&w=1000&q=85" alt="Superficies en piedra, granito y cuarzo">

                <div class="card-overlay">

                    <h3>Cubiertas & Piedra</h3>

                    <p>
                        Integración de superficies en granito,
                        cuarzo y piedras naturales.
                    </p>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- MATERIALES -->

<section class="combinations" id="materiales">

    <div class="container">

        <div class="section-title">

            <small>Texturas y Combinaciones</small>

            <h2 style="color: white;">La Armonía de los Materiales</h2>

            <p style="color: #ccc;">
                Seleccionamos maderas nobles y piedras de alta calidad para crear contrastes visuales, táctiles y elegantes.
            </p>

        </div>

        <div class="combination-grid">

            <div class="material">
                <img src="https://images.unsplash.com/photo-1546484475-7f7bd55792da?auto=format&fit=crop&w=600&q=85" alt="Madera de Nogal">
                <span>Nogal Cálido</span>
            </div>

            <div class="material">
                <img src="https://images.unsplash.com/photo-1618221118493-9cfa1a1c00da?auto=format&fit=crop&w=600&q=85" alt="Cuarzo y Mármol Calacatta">
                <span>Cuarzo & Piedra</span>
            </div>

            <div class="material">
                <img src="https://images.unsplash.com/photo-1513694203232-719a280e022f?auto=format&fit=crop&w=600&q=85" alt="Madera de Encino">
                <span>Encino Natural</span>
            </div>

            <div class="material">
                <img src="https://images.unsplash.com/photo-1600585152220-90363fe7e115?auto=format&fit=crop&w=600&q=85" alt="Granito Oscuro">
                <span>Granito & Tonos Oscuros</span>
            </div>

        </div>

    </div>

</section>


<!-- PROYECTOS -->

<section id="proyectos">

    <div class="container">

        <div class="section-title">

            <small>Galería de Trabajos</small>

            <h2>Proyectos Recientes</h2>

            <p>
                Una muestra de nuestras entregas residenciales en el sur de Tamaulipas y región.
            </p>

        </div>

        <div class="projects">

            <div class="project">
                <img src="https://images.unsplash.com/photo-1600585154526-990dced4db0d?auto=format&fit=crop&w=1200&q=85" alt="Cocina integral de lujo">
            </div>

            <div class="project">
                <img src="https://images.unsplash.com/photo-1600566752355-35792bedcfea?auto=format&fit=crop&w=800&q=85" alt="Isla de cocina con barra de cuarzo">
            </div>

            <div class="project">
                <img src="https://images.unsplash.com/photo-1600210492486-724fe5c67fb0?auto=format&fit=crop&w=800&q=85" alt="Detalle de carpintería fina">
            </div>

            <div class="project">
                <img src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c?auto=format&fit=crop&w=800&q=85" alt="Mueble de madera para cocina">
            </div>

            <div class="project">
                <img src="https://images.unsplash.com/photo-1600566753190-17f0baa2a6c3?auto=format&fit=crop&w=800&q=85" alt="Mobiliario residencial integrado">
            </div>

        </div>

    </div>

</section>


<!-- ZONAS DE COBERTURA -->

<section class="zones">

    <div class="container">

        <div class="section-title">

            <small>Cobertura de Servicio</small>

            <h2>Presencia Regional</h2>

            <p>
                Atendemos proyectos de diseño, fabricación e instalación en las siguientes zonas:
            </p>

        </div>

        <div class="zones-grid">

            <div class="zone">
                <h3>Sur de Tamaulipas</h3>
                <p>Tampico, Ciudad Madero y Altamira.</p>
            </div>

            <div class="zone">
                <h3>Norte de Veracruz</h3>
                <p>Pánuco, Pueblo Viejo, Poza Rica y alrededores.</p>
            </div>

            <div class="zone">
                <h3>Huasteca Potosina</h3>
                <p>Ciudad Valles y municipios vecinos de la región.</p>
            </div>

        </div>

    </div>

</section>


<!-- CALL TO ACTION -->

<section class="cta">

    <div class="container">

        <h2>¿Tienes un proyecto en mente?</h2>

        <p>
            Transformamos tus ideas en planos y materiales de alta calidad adaptados a tu espacio.
        </p>

        <div class="buttons" style="margin-top: 30px;">
            <!-- SUSTITUIR 'TUNUMERO' POR TU NÚMERO REAL -->
            <a class="btn primary" href="https://wa.me/TUNUMERO" target="_blank" rel="noopener">
                INICIAR COTIZACIÓN
            </a>
        </div>

    </div>

</section>


<!-- CONTACTO -->

<section id="contacto">

    <div class="container contact-grid">

        <div class="contact-info">

            <small>Contacto Directo</small>

            <h2>Hablemos de tu Espacio</h2>

            <p>
                Déjanos tus datos o escríbenos directamente para programar una cita de valoración técnica o diseño.
            </p>

            <p>
                <strong>Ubicación:</strong> Zona Metropolitana de Tampico, Tam.<br>
                <strong>Atención:</strong> Lunes a Sábado de 9:00 AM a 6:00 PM
            </p>

        </div>

        <div>

            <form action="#" method="POST" onsubmit="event.preventDefault(); alert('¡Gracias! Nos pondremos en contacto contigo pronto.');">

                <input type="text" name="nombre" placeholder="Nombre completo" required>

                <input type="email" name="email" placeholder="Correo electrónico" required>

                <input type="tel" name="telefono" placeholder="Teléfono de contacto" required>

                <textarea name="mensaje" placeholder="Platícanos sobre tu proyecto (ej. cocina integral en Tampico, vestidor, etc.)" required></textarea>

                <button type="submit">ENVIAR MENSAJE</button>

            </form>

        </div>

    </div>

</section>


<!-- FOOTER -->

<footer>

    <div class="container">

        <h2>IZIA</h2>

        <p>ESPACIOS EN MADERA &copy; 2026. Todos los derechos reservados.</p>

    </div>

</footer>


<!-- BOTÓN FLOTANTE DE CONTACTO -->

<div class="floating" id="floatingMenu">

    <div class="float-menu">

        <!-- SUSTITUIR 'TUNUMERO' Y REDES SOCIALES POR LAS TUYAS -->
        <a href="https://wa.me/TUNUMERO" class="float-item whatsapp" title="WhatsApp" target="_blank" rel="noopener">
            <i class="fa-brands fa-whatsapp"></i>
        </a>

        <a href="https://facebook.com" class="float-item facebook" title="Facebook" target="_blank" rel="noopener">
            <i class="fa-brands fa-facebook-f"></i>
        </a>

        <a href="mailto:contacto@izia.com" class="float-item email" title="Correo Electrónico">
            <i class="fa-regular fa-envelope"></i>
        </a>

    </div>

    <button class="float-main" aria-label="Contacto flotante" onclick="toggleFloatingMenu()">
        <i class="fa-solid fa-plus"></i>
    </button>

</div>


<!-- SCRIPTS -->

<script>
    function toggleMenu() {
        const menu = document.getElementById('menu');
        menu.classList.toggle('active');
    }

    function toggleFloatingMenu() {
        const floating = document.getElementById('floatingMenu');
        floating.classList.toggle('active');
    }

    // Cierre automático del menú móvil al seleccionar cualquier enlace
    document.querySelectorAll('.menu a').forEach(link => {
        link.addEventListener('click', () => {
            document.getElementById('menu').classList.remove('active');
        });
    });
</script>

</body>
</html>

