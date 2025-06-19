---
layout: landing # Ahora usamos el layout 'landing'
title: Sobre Mí - Guillermo
subtitle: Creativo Digital | Mi Experiencia, Habilidades y Pasiones
image: assets/images/pic07.jpg # Puedes usar una imagen tuya o una representativa
alt: Retrato de Guillermo o icono personal
date: 2024-06-20 10:00:00 +0200 # Fecha de actualización de la página
permalink: /sobre-mi/ # Definimos una URL clara para tu página Sobre Mí
nav-menu: true # Mantener el menú de navegación si el layout landing lo requiere
---

<div id="main">

<section id="one">
    <div class="inner">
        <header class="major">
            <h2>Hola, soy Guillermo.</h2>
        </header>
        <p>Soy un **Creativo Digital** apasionado por transformar ideas en experiencias visuales y funcionales. Mi trayectoria abarca el diseño gráfico, la comunicación estratégica y el desarrollo de proyectos creativos que buscan conectar y generar impacto. Siempre en constante aprendizaje, disfruto explorando nuevas herramientas y técnicas para dar vida a soluciones innovadoras.</p>
    </div>
</section>

<section id="two" class="spotlights">
    <section>
        <a href="{{ site.baseurl }}/proyectos/" class="image">
            <img src="{{ site.baseurl }}/assets/images/pic08.jpg" alt="Imagen representativa de proyectos" data-position="center center" />
        </a>
        <div class="content">
            <div class="inner">
                <header class="major">
                    <h3>Mis Proyectos</h3>
                </header>
                <p>Descubre mi trabajo más reciente en diseño web, branding, campañas visuales y proyectos integrales. Cada uno es un reflejo de mi pasión por la creatividad y la resolución de problemas.</p>
                <ul class="actions">
                    <li><a href="{{ site.baseurl }}/proyectos/" class="button">Ver Proyectos</a></li>
                </ul>
            </div>
        </div>
    </section>
    <section>
        <a href="{{ site.baseurl }}/posts/" class="image">
            <img src="{{ site.baseurl }}/assets/images/pic09.jpg" alt="Imagen representativa de posts/artículos" data-position="top center" />
        </a>
        <div class="content">
            <div class="inner">
                <header class="major">
                    <h3>Artículos y Reflexiones</h3>
                </header>
                <p>En este espacio comparto mis pensamientos, análisis y pequeños tutoriales sobre diseño, tendencias digitales y el proceso creativo. Un lugar para profundizar y aprender.</p>
                <ul class="actions">
                    <li><a href="{{ site.baseurl }}/posts/" class="button">Leer Artículos</a></li>
                </ul>
            </div>
        </div>
    </section>
    <section>
        <a href="{{ site.baseurl }}/cv/" class="image">
            <img src="{{ site.baseurl }}/assets/images/pic10.jpg" alt="Imagen representativa de CV" data-position="25% 25%" />
        </a>
        <div class="content">
            <div class="inner">
                <header class="major">
                    <h3>Mi Trayectoria Profesional</h3>
                </header>
                <p>Explora mi experiencia profesional, habilidades clave, formación académica y las herramientas que domino. Un vistazo detallado a mi perfil y lo que puedo ofrecer.</p>
                <ul class="actions">
                    <li><a href="{{ site.baseurl }}/cv/" class="button">Ver CV</a></li>
                </ul>
            </div>
        </div>
    </section>
</section>

<section id="three">
    <div class="inner">
        <header class="major">
            <h2>¿Hablamos?</h2>
        </header>
        <p>Si te interesa colaborar en un proyecto, tienes alguna pregunta o simplemente quieres saludar, no dudes en contactarme. Estoy abierto a nuevas oportunidades y conexiones.</p>
        <ul class="actions">
            <li><a href="mailto:{{ site.email }}" class="button next">Enviar un email</a></li>
        </ul>
    </div>
</section>

</div>