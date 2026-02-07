<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Amparo Pozo - Estudio de interiorismo y decoración en Madrid. Diseño de interiores exclusivo para viviendas de lujo, oficinas y locales comerciales. Reformas integrales con arquitectura emocional.">
    <meta name="keywords" content="interiorista Madrid, diseño de interiores, decoradora Madrid, reformas integrales, arquitectura interior, interiorismo lujo, Amparo Pozo">
    <meta name="author" content="Amparo Pozo Interiorismo">
    <meta name="robots" content="index, follow">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://amparopozo.es">
    <meta property="og:title" content="Amparo Pozo | Interiorismo y Decoración de Lujo en Madrid">
    <meta property="og:description" content="Estudio de interiorismo en Madrid especializado en arquitectura emocional. Transformamos espacios ordinarios en experiencias extraordinarias.">
    <meta property="og:image" content="https://amparopozo.es/images/og-image.jpg">

    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://amparopozo.es">
    <meta property="twitter:title" content="Amparo Pozo | Interiorismo de Vanguardia en Madrid">
    <meta property="twitter:description" content="Diseño de interiores exclusivo que despierta emociones. Reformas integrales con sello propio.">
    <meta property="twitter:image" content="https://amparopozo.es/images/twitter-image.jpg">

    <!-- Canonical URL -->
    <link rel="canonical" href="https://amparopozo.es">
    
    <title>Amparo Pozo | Interiorismo y Decoración de Lujo en Madrid</title>
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --color-primary: #1a1a1a;
            --color-secondary: #c9a962;
            --color-accent: #f4f1ea;
            --color-text: #333;
            --color-light: #fff;
            --font-heading: 'Playfair Display', serif;
            --font-body: 'Montserrat', sans-serif;
        }

        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,400;0,600;1,400&display=swap');

        body {
            font-family: var(--font-body);
            color: var(--color-text);
            line-height: 1.6;
            overflow-x: hidden;
            background-color: var(--color-light);
        }

        /* Scroll Progress Bar */
        .progress-bar {
            position: fixed;
            top: 0;
            left: 0;
            height: 3px;
            background: var(--color-secondary);
            z-index: 1001;
            transition: width 0.1s;
        }

        /* Navigation */
        nav {
            position: fixed;
            top: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            z-index: 1000;
            padding: 1rem 5%;
            box-shadow: 0 2px 20px rgba(0,0,0,0.05);
            transition: all 0.3s ease;
        }

        nav.scrolled {
            padding: 0.5rem 5%;
        }

        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: var(--font-heading);
            font-size: 1.8rem;
            font-weight: 600;
            color: var(--color-primary);
            text-decoration: none;
            letter-spacing: 2px;
        }

        .logo span {
            color: var(--color-secondary);
        }

        .nav-links {
            display: flex;
            gap: 2.5rem;
            list-style: none;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--color-primary);
            font-weight: 500;
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 1px;
            position: relative;
            transition: color 0.3s;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--color-secondary);
            transition: width 0.3s;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .mobile-menu {
            display: none;
            flex-direction: column;
            gap: 5px;
            cursor: pointer;
        }

        .mobile-menu span {
            width: 25px;
            height: 2px;
            background: var(--color-primary);
            transition: 0.3s;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            background: linear-gradient(135deg, #f5f5f5 0%, #e8e8e8 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -10%;
            width: 800px;
            height: 800px;
            background: radial-gradient(circle, rgba(201,169,98,0.1) 0%, transparent 70%);
            animation: float 20s infinite ease-in-out;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            50% { transform: translate(-30px, -30px) rotate(180deg); }
        }

        .hero-content {
            text-align: center;
            z-index: 2;
            max-width: 900px;
            padding: 0 2rem;
            animation: fadeInUp 1s ease;
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .hero h1 {
            font-family: var(--font-heading);
            font-size: clamp(2.5rem, 5vw, 4.5rem);
            color: var(--color-primary);
            margin-bottom: 1.5rem;
            line-height: 1.2;
            font-weight: 400;
        }

        .hero h1 em {
            color: var(--color-secondary);
            font-style: italic;
        }

        .hero-subtitle {
            font-size: 1.2rem;
            color: #666;
            margin-bottom: 2rem;
            font-weight: 300;
            letter-spacing: 2px;
        }

        .hero-description {
            font-size: 1.1rem;
            color: #555;
            max-width: 700px;
            margin: 0 auto 3rem;
            line-height: 1.8;
        }

        .cta-button {
            display: inline-block;
            padding: 1rem 3rem;
            background: var(--color-primary);
            color: var(--color-light);
            text-decoration: none;
            font-weight: 500;
            letter-spacing: 2px;
            text-transform: uppercase;
            font-size: 0.9rem;
            transition: all 0.3s;
            border: 2px solid var(--color-primary);
            position: relative;
            overflow: hidden;
        }

        .cta-button::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: var(--color-secondary);
            transition: left 0.3s;
            z-index: -1;
        }

        .cta-button:hover::before {
            left: 0;
        }

        .cta-button:hover {
            color: var(--color-primary);
            border-color: var(--color-secondary);
        }

        /* Cities Marquee */
        .cities-marquee {
            background: var(--color-primary);
            color: var(--color-light);
            padding: 1rem 0;
            overflow: hidden;
            white-space: nowrap;
            position: relative;
        }

        .marquee-content {
            display: inline-block;
            animation: marquee 30s linear infinite;
        }

        @keyframes marquee {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }

        .cities-marquee span {
            margin: 0 2rem;
            font-size: 0.85rem;
            letter-spacing: 2px;
            opacity: 0.8;
        }

        /* About Section */
        .about {
            padding: 8rem 5%;
            background: var(--color-light);
            position: relative;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }

        .section-tag {
            color: var(--color-secondary);
            text-transform: uppercase;
            letter-spacing: 3px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-bottom: 1rem;
            display: block;
        }

        .section-title {
            font-family: var(--font-heading);
            font-size: clamp(2rem, 4vw, 3rem);
            color: var(--color-primary);
            margin-bottom: 1.5rem;
            font-weight: 400;
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text h3 {
            font-family: var(--font-heading);
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: var(--color-primary);
            font-weight: 400;
        }

        .about-text p {
            margin-bottom: 1.5rem;
            color: #555;
            line-height: 1.8;
            font-size: 1.05rem;
        }

        .about-text strong {
            color: var(--color-primary);
            font-weight: 600;
        }

        .quote-box {
            background: var(--color-accent);
            padding: 2.5rem;
            border-left: 4px solid var(--color-secondary);
            margin: 2rem 0;
            position: relative;
            font-style: italic;
            font-family: var(--font-heading);
            font-size: 1.2rem;
            color: var(--color-primary);
            line-height: 1.8;
        }

        .quote-box::before {
            content: '"';
            font-size: 4rem;
            color: var(--color-secondary);
            position: absolute;
            top: -10px;
            left: 20px;
            opacity: 0.3;
        }

        .quote-author {
            display: block;
            margin-top: 1.5rem;
            font-style: normal;
            font-family: var(--font-body);
            font-size: 0.9rem;
            color: #666;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        .about-image {
            position: relative;
            overflow: hidden;
            box-shadow: 30px 30px 0 var(--color-secondary);
        }

        .about-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: transform 0.5s;
        }

        .about-image:hover img {
            transform: scale(1.05);
        }

        /* Features Grid */
        .features {
            padding: 6rem 5%;
            background: var(--color-accent);
        }

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
        }

        .feature-card {
            text-align: center;
            padding: 2.5rem;
            background: var(--color-light);
            transition: transform 0.3s, box-shadow 0.3s;
            border-bottom: 3px solid transparent;
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
            border-bottom-color: var(--color-secondary);
        }

        .feature-icon {
            width: 60px;
            height: 60px;
            background: var(--color-secondary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1.5rem;
            color: var(--color-light);
            font-size: 1.5rem;
        }

        .feature-card h3 {
            font-family: var(--font-heading);
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--color-primary);
        }

        .feature-card p {
            color: #666;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        /* Services Section */
        .services {
            padding: 8rem 5%;
            background: var(--color-light);
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 4rem;
        }

        .service-card {
            padding: 3rem;
            border: 1px solid #eee;
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: var(--color-primary);
            transform: translateY(100%);
            transition: transform 0.3s;
            z-index: 0;
        }

        .service-card:hover::before {
            transform: translateY(0);
        }

        .service-card:hover h3,
        .service-card:hover p {
            color: var(--color-light);
        }

        .service-card > * {
            position: relative;
            z-index: 1;
        }

        .service-card h3 {
            font-family: var(--font-heading);
            font-size: 1.5rem;
            margin-bottom: 1rem;
            color: var(--color-primary);
            transition: color 0.3s;
        }

        .service-card p {
            color: #666;
            line-height: 1.7;
            transition: color 0.3s;
        }

        .service-number {
            font-size: 3rem;
            font-weight: 700;
            color: var(--color-secondary);
            opacity: 0.3;
            position: absolute;
            top: 1rem;
            right: 1.5rem;
            font-family: var(--font-heading);
        }

        /* Process Section */
        .process {
            padding: 8rem 5%;
            background: var(--color-primary);
            color: var(--color-light);
        }

        .process .section-title {
            color: var(--color-light);
        }

        .process-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
            position: relative;
        }

        .process-steps::before {
            content: '';
            position: absolute;
            top: 40px;
            left: 10%;
            right: 10%;
            height: 2px;
            background: rgba(201,169,98,0.3);
            z-index: 0;
        }

        .step {
            text-align: center;
            position: relative;
            z-index: 1;
        }

        .step-number {
            width: 80px;
            height: 80px;
            background: var(--color-secondary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 1.5rem;
            font-family: var(--font-heading);
            font-size: 1.5rem;
            font-weight: 600;
            color: var(--color-primary);
            border: 4px solid var(--color-primary);
        }

        .step h3 {
            font-family: var(--font-heading);
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: var(--color-light);
        }

        .step p {
            color: #aaa;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        /* Why Choose Us */
        .why-us {
            padding: 8rem 5%;
            background: var(--color-light);
        }

        .why-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 3rem;
            margin-top: 4rem;
        }

        .why-item {
            display: flex;
            gap: 1.5rem;
            align-items: flex-start;
        }

        .why-icon {
            min-width: 50px;
            height: 50px;
            background: var(--color-accent);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            color: var(--color-secondary);
        }

        .why-content h3 {
            font-family: var(--font-heading);
            font-size: 1.3rem;
            margin-bottom: 0.5rem;
            color: var(--color-primary);
        }

        .why-content p {
            color: #666;
            font-size: 0.95rem;
            line-height: 1.6;
        }

        /* Contact CTA */
        .contact-cta {
            padding: 6rem 5%;
            background: var(--color-secondary);
            text-align: center;
            color: var(--color-light);
        }

        .contact-cta h2 {
            font-family: var(--font-heading);
            font-size: clamp(2rem, 4vw, 3rem);
            margin-bottom: 1.5rem;
        }

        .contact-cta p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
            opacity: 0.9;
        }

        .contact-cta .cta-button {
            background: var(--color-light);
            color: var(--color-primary);
            border-color: var(--color-light);
        }

        .contact-cta .cta-button::before {
            background: var(--color-primary);
        }

        .contact-cta .cta-button:hover {
            color: var(--color-light);
            border-color: var(--color-primary);
        }

        /* Footer */
        footer {
            background: var(--color-primary);
            color: var(--color-light);
            padding: 4rem 5% 2rem;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            max-width: 1200px;
            margin: 0 auto 3rem;
        }

        .footer-col h4 {
            font-family: var(--font-heading);
            font-size: 1.2rem;
            margin-bottom: 1.5rem;
            color: var(--color-secondary);
        }

        .footer-col p,
        .footer-col a {
            color: #aaa;
            text-decoration: none;
            line-height: 1.8;
            transition: color 0.3s;
        }

        .footer-col a:hover {
            color: var(--color-secondary);
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #333;
            color: #666;
            font-size: 0.9rem;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .mobile-menu {
                display: flex;
            }

            .about-grid {
                grid-template-columns: 1fr;
            }

            .about-image {
                box-shadow: 15px 15px 0 var(--color-secondary);
                order: -1;
            }

            .process-steps::before {
                display: none;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }
        }

        /* Animations on scroll */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s, transform 0.8s;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Progress Bar -->
    <div class="progress-bar" id="progressBar"></div>

    <!-- Navigation -->
    <nav id="navbar">
        <div class="nav-container">
            <a href="#" class="logo">Amparo <span>Pozo</span></a>
            <ul class="nav-links">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#estudio">Estudio</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#proceso">Proceso</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
            <div class="mobile-menu">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="hero-content">
            <h1>Diseño de Interiores que <em>Transforma</em> Realidades</h1>
            <p class="hero-subtitle">Interiorismo de Vanguardia en Madrid</p>
            <p class="hero-description">
                Nuestros proyectos de arquitectura interior elevan el valor de tu inmueble y potencian tu negocio. 
                Una sola oportunidad para causar una impresión indeleble. Es el momento de conectar con nuevas 
                oportunidades, impulsar tus resultados o disfrutar de un hogar que parece salido de las páginas 
                de una revista de decoración en Madrid.
            </p>
            <a href="#contacto" class="cta-button">Descubre Nuestro Método</a>
        </div>
    </section>

    <!-- Cities Marquee -->
    <div class="cities-marquee">
        <div class="marquee-content">
            <span>Madrid</span><span>Barcelona</span><span>Valencia</span><span>Sevilla</span>
            <span>Málaga</span><span>Marbella</span><span>Bilbao</span><span>Zaragoza</span>
            <span>Palma de Mallorca</span><span>Ibiza</span><span>Alicante</span><span>Murcia</span>
            <span>Toledo</span><span>Salamanca</span><span>Valladolid</span><span>Granada</span>
            <span>Madrid</span><span>Barcelona</span><span>Valencia</span><span>Sevilla</span>
            <span>Málaga</span><span>Marbella</span><span>Bilbao</span><span>Zaragoza</span>
        </div>
    </div>

    <!-- About Section -->
    <section class="about" id="estudio">
        <div class="container">
            <div class="section-header fade-in">
                <span class="section-tag">Estudio de Interiorismo</span>
                <h2 class="section-title">Arquitectura Emocional y Diseño Estratégico</h2>
            </div>
            
            <div class="about-grid">
                <div class="about-text fade-in">
                    <h3>Un Estudio de Interiorismo en Madrid con Proyección Nacional</h3>
                    <p>
                        <strong>Estudio de interiorismo en Madrid</strong>, con sede operativa en la capital, 
                        dirigido por <em>Amparo Pozo, arquitecta de interiores y asesora de decoración</em> 
                        con más de una década de trayectoria profesional.
                    </p>
                    <p>
                        Esta <strong>interiorista en Madrid</strong> aporta un enfoque diferencial y 
                        completamente personalizado a cada encargo. Gracias a su visión creativa y 
                        dominio técnico, <em>Amparo Pozo Estudio</em> se ha consolidado como referente 
                        en el sector del <strong>diseño de interiores en Madrid</strong>, concebiendo 
                        ambientes donde la estética, la funcionalidad y la emoción coexisten en perfecta 
                        armonía.
                    </p>
                    <p>
                        Si buscas <strong>interioristas en Madrid</strong> capaces de metamorfosear 
                        tu espacio vital o laboral, Amparo Pozo representa la elección idónea para 
                        materializar tus visiones con un sello distintivo de sofisticación y excelencia técnica.
                    </p>
                    
                    <div class="quote-box">
                        Nuestra misión es desafiar lo convencional, buscar el impacto visual genuino 
                        y conseguir que cada estancia evoque sentimientos profundos y cree recuerdos 
                        imborrables. No nos conformamos con diseñar; aspiramos a que nos recuerden 
                        cada vez que alguien pisa uno de nuestros espacios. Pretendemos llevar la 
                        <strong>arquitectura de interiores</strong> a su máxima expresión. Por ello, 
                        abrazamos el <strong>interiorismo creativo</strong>, el <strong>diseño estratégico</strong> 
                        y el <strong>interiorismo experiencial</strong>.
                        <span class="quote-author">— Amparo Pozo, directora creativa</span>
                    </div>
                </div>
                
                <div class="about-image fade-in">
                    <img src="https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?w=800&q=80" 
                         alt="Proyecto de interiorismo de Amparo Pozo - Diseño de salón moderno">
                </div>
            </div>
        </div>
    </section>

    <!-- Features Section -->
    <section class="features">
        <div class="container">
            <div class="section-header fade-in">
                <span class="section-tag">Nuestra Filosofía</span>
                <h2 class="section-title">Interiorismo Madrid</h2>
                <p style="color: #666; max-width: 600px; margin: 0 auto;">Resultados que superan expectativas, garantizados por nuestro método de trabajo</p>
            </div>
            
            <div class="features-grid">
                <div class="feature-card fade-in">
                    <div class="feature-icon">📐</div>
                    <h3>Análisis Espacial Exhaustivo</h3>
                    <p>Nuestro equipo de interioristas en Madrid examina y optimiza cada centímetro disponible, maximizando el potencial de cualquier estancia.</p>
                </div>
                
                <div class="feature-card fade-in">
                    <div class="feature-icon">✨</div>
                    <h3>Diseños que Captivan</h3>
                    <p>Interiorismo estratégico y sensorial para cada encargo, potenciando juegos visuales y experiencias multisensoriales únicas.</p>
                </div>
                
                <div class="feature-card fade-in">
                    <div class="feature-icon">🛡️</div>
                    <h3>Cadena de Valor Inmejorable</h3>
                    <p>Reforma integral en Madrid supervisada de principio a fin. Tu tranquilidad es nuestra prioridad absoluta.</p>
                </div>
                
                <div class="feature-card fade-in">
                    <div class="feature-icon">🎯</div>
                    <h3>Objetivo Definido</h3>
                    <p>Crear espacios absolutamente personalizados para clientes exigentes, visionarios y amantes del diseño diferenciado.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="servicios">
        <div class="container">
            <div class="section-header fade-in">
                <span class="section-tag">Servicios Especializados</span>
                <h2 class="section-title">Servicio de Interiorismo en Madrid</h2>
                <p style="color: #666; max-width: 700px; margin: 0 auto;">
                    ¿Deseas conocer nuestro universo creativo? Explora los <strong>servicios de interiorismo</strong> 
                    que desarrollamos y descubre la versatilidad de cada <strong>proyecto de diseño</strong>.
                </p>
            </div>
            
            <div class="services-grid">
                <div class="service-card fade-in">
                    <span class="service-number">01</span>
                    <h3>Arquitectura Interior y Diseño Estratégico</h3>
                    <p>Ejecutamos reformas integrales completas, iniciando con un proyecto de arquitectura de interiores y planificación estratégica. Identificamos las soluciones óptimas para la distribución espacial, diseñamos el sistema de iluminación, elaboramos planos de instalaciones, seleccionamos materiales de alta gama y gestionamos el mobiliario y tapizados personalizados.</p>
                </div>
                
                <div class="service-card fade-in">
                    <span class="service-number">02</span>
                    <h3>Decoración de Interiores Premium</h3>
                    <p>¿Contemplas renovar los ambientes de tu residencia? Ofrecemos un servicio de decoración de interiores exclusivo. Somos distribuidores directos de prestigiosas marcas italianas, portuguesas y españolas. Disponemos además de taller propio para fabricación de mobiliario a medida y curamos la selección de textiles e iluminación para crear atmósferas perfectas.</p>
                </div>
                
                <div class="service-card fade-in">
                    <span class="service-number">03</span>
                    <h3>Estudio de Optimización Espacial</h3>
                    <p>¿Anhelas explotar el máximo potencial de tu vivienda? Realizamos un análisis profundo del espacio, ya sea en obra nueva, proyecto futuro o reforma. Optimizamos almacenamiento y distribución. No existen espacios reducidos, únicamente espacios mal planificados.</p>
                </div>
                
                <div class="service-card fade-in">
                    <span class="service-number">04</span>
                    <h3>Servicios Online: Asesoría y Decoración</h3>
                    <p>¿Imaginas transformar radicalmente un espacio únicamente mediante tu dispositivo móvil? Es posible gracias a nuestros planes de decoración online. Descubre cómo funciona nuestra metodología digital.</p>
                </div>
                
                <div class="service-card fade-in">
                    <span class="service-number">05</span>
                    <h3>Diseño de Hostelería y Retail</h3>
                    <p>Especialistas en proyectos para el sector hospitality, diseño de oficinas corporativas, locales comerciales con identidad propia, viviendas de lujo y diseño de fachadas para residencias exclusivas.</p>
                </div>
                
                <div class="service-card fade-in">
                    <span class="service-number">06</span>
                    <h3>Interiorismo Emocional</h3>
                    <p>Proyectamos espacios residenciales enfocados en generar bienestar y emociones positivas. Cada rincón está pensado para conectar contigo a nivel sensorial y emocional, creando hogares que sanan y energizan.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section class="process" id="proceso">
        <div class="container">
            <div class="section-header fade-in">
                <span class="section-tag" style="color: var(--color-secondary);">Metodología de Trabajo</span>
                <h2 class="section-title">Empresas de Interiorismo Madrid</h2>
                <p style="color: #aaa; max-width: 600px; margin: 0 auto;">Un proceso estructurado para resultados excepcionales</p>
            </div>
            
            <div class="process-steps">
                <div class="step fade-in">
                    <div class="step-number">01</div>
                    <h3>Plan de Requerimientos</h3>
                    <p>Contacta con nuestra empresa de interiorismo en Madrid. Envíanos planos o fotografías del espacio a evaluar, especificando tus necesidades y aspiraciones.</p>
                </div>
                
                <div class="step fade-in">
                    <div class="step-number">02</div>
                    <h3>Reunión Estratégica</h3>
                    <p>Identificamos los elementos clave para potenciar tu espacio y elevarlo al máximo nivel de excelencia y funcionalidad.</p>
                </div>
                
                <div class="step fade-in">
                    <div class="step-number">03</div>
                    <h3>Desarrollo Creativo</h3>
                    <p>Iniciamos la fase de conceptualización y diseño del interior y/o exterior según tus preferencias y nuestro criterio profesional.</p>
                </div>
                
                <div class="step fade-in">
                    <div class="step-number">04</div>
                    <h3>Entrega del Proyecto</h3>
                    <p>Presentamos la propuesta definitiva. Tras tu aprobación, proporcionamos toda la documentación técnica necesaria para iniciar la ejecución.</p>
                </div>
                
                <div class="step fade-in">
                    <div class="step-number">05</div>
                    <h3>Ejecución de Obra</h3>
                    <p>Nos adaptamos a tus requerimientos específicos. Coordinamos la obra para garantizar que el proyecto se materialice fiel al diseño aprobado.</p>
                </div>
                
                <div class="step fade-in">
                    <div class="step-number">06</div>
                    <h3>Servicio Llave en Mano</h3>
                    <p>Con nuestro servicio integral, nos ocupamos de todo para que el proyecto se ejecute exactamente como lo visualizaste, sin preocupaciones. Solo te quedará disfrutarlo.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Why Choose Us -->
    <section class="why-us">
        <div class="container">
            <div class="section-header fade-in">
                <span class="section-tag">Ventajas Competitivas</span>
                <h2 class="section-title">Amparo Pozo Estudio</h2>
                <p style="color: #666; max-width: 600px; margin: 0 auto;">¿Por qué seleccionarnos como tus interioristas de confianza?</p>
            </div>
            
            <div class="why-grid">
                <div class="why-item fade-in">
                    <div class="why-icon">🏆</div>
                    <div class="why-content">
                        <h3>Exclusividad Absoluta</h3>
                        <p>Nuestra devoción por la excelencia se manifiesta en cada proyecto. No existirá otro espacio idéntico al tuyo. Serás único e irrepetible.</p>
                    </div>
                </div>
                
                <div class="why-item fade-in">
                    <div class="why-icon">⚡</div>
                    <div class="why-content">
                        <h3>Diseño Extraordinario</h3>
                        <p>Nuestro valor añadido ("Extra") supone el salto cualitativo de lo ordinario a lo verdaderamente excepcional.</p>
                    </div>
                </div>
                
                <div class="why-item fade-in">
                    <div class="why-icon">✓</div>
                    <div class="why-content">
                        <h3>Resultados Garantizados</h3>
                        <p>Más de 500 clientes satisfechos respaldan nuestra trayectoria. Contamos con los mejores profesionales del interiorismo en Madrid.</p>
                    </div>
                </div>
                
                <div class="why-item fade-in">
                    <div class="why-icon">💎</div>
                    <div class="why-content">
                        <h3>Materiales de Élite</h3>
                        <p>Colaboramos con las firmas más prestigiosas en materiales, mobiliario y textiles para cada intervención.</p>
                    </div>
                </div>
                
                <div class="why-item fade-in">
                    <div class="why-icon">🥽</div>
                    <div class="why-content">
                        <h3>Tecnología Inmersiva</h3>
                        <p>Empleamos Realidad Virtual para que experimentes en primera persona cómo será tu espacio antes de construirlo.</p>
                    </div>
                </div>
                
                <div class="why-item fade-in">
                    <div class="why-icon">🔄</div>
                    <div class="why-content">
                        <h3>Filosofía Kaizen</h3>
                        <p>La mejora continua como forma de vida constituye nuestro sello distintivo y compromiso con la evolución permanente.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact CTA -->
    <section class="contact-cta" id="contacto">
        <div class="container">
            <h2>¿Listo para Transformar tu Espacio?</h2>
            <p>Conversemos sobre tu proyecto. La primera consulta es gratuita y sin compromiso.</p>
            <a href="mailto:info@amparopozo.es" class="cta-button">Iniciar Conversación</a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="footer-grid">
            <div class="footer-col">
                <h4>Amparo Pozo</h4>
                <p>Estudio de interiorismo y arquitectura emocional en Madrid. Transformamos espacios ordinarios en experiencias extraordinarias desde 2012.</p>
            </div>
            
            <div class="footer-col">
                <h4>Servicios</h4>
                <p><a href="#">Arquitectura Interior</a></p>
                <p><a href="#">Decoración Premium</a></p>
                <p><a href="#">Reformas Integrales</a></p>
                <p><a href="#">Consultoría Online</a></p>
            </div>
            
            <div class="footer-col">
                <h4>Contacto</h4>
                <p>Madrid, España</p>
                <p><a href="mailto:info@amparopozo.es">info@amparopozo.es</a></p>
                <p><a href="tel:+34123456789">+34 123 456 789</a></p>
            </div>
            
            <div class="footer-col">
                <h4>Legal</h4>
                <p><a href="#">Política de Privacidad</a></p>
                <p><a href="#">Aviso Legal</a></p>
                <p><a href="#">Política de Cookies</a></p>
            </div>
        </div>
        
        <div class="footer-bottom">
            <p>&copy; 2024 Amparo Pozo Interiorismo. Todos los derechos reservados.</p>
        </div>
    </footer>

    <script>
        // Progress Bar
        window.onscroll = function() {
            let winScroll = document.body.scrollTop || document.documentElement.scrollTop;
            let height = document.documentElement.scrollHeight - document.documentElement.clientHeight;
            let scrolled = (winScroll / height) * 100;
            document.getElementById("progressBar").style.width = scrolled + "%";
            
            // Navbar effect
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        };

        // Intersection Observer for fade-in animations
        const observerOptions = {
            root: null,
            rootMargin: '0px',
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach((el) => observer.observe(el));

        // Smooth scroll for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>
