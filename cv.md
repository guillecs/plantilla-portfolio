---
layout: landing # Ahora usamos el layout 'landing'
title: Mi Currículum Vitae
subtitle: Descarga mi CV completo en formato PDF.
image: assets/images/pic04.jpg # Mantén la imagen que tenías o usa una más adecuada para CV
alt: Icono de currículum o documento
date: 2025-06-20 10:38:07 +0200 # Fecha de última actualización de esta página
permalink: /cv/ # La URL para esta página
nav-menu: true # Mantener el menú de navegación si el layout landing lo requiere
---

<div id="main">

    <section id="one">
        <div class="inner">
            <header class="major">
                <h2>Guillermo - Creativo Digital</h2>
            </header>
            <p>Soy un **Creativo Digital** apasionado por [menciona tu principal pasión, ej. el diseño de experiencias, la comunicación visual, el desarrollo web]. Aquí puedes encontrar un resumen de mis habilidades y mi experiencia. Para una visión completa de mi trayectoria profesional, incluyendo detalles sobre mi experiencia, formación académica y proyectos específicos, te invito a **descargar mi CV completo en formato PDF**.</p>

            <ul class="actions">
                <li><a href="{{ site.baseurl }}/assets/cv/tu-cv-nombre.pdf" class="button next icon solid fa-download">Descargar CV en PDF</a></li>
            </ul>

            <p class="small-text"><i>Última actualización del CV: {{ page.date | date: "%d/%m/%Y" }}</i></p>
        </div>
    </section>

    <section id="three">
        <div class="inner">
            <header class="major">
                <h2>¿Hablamos?</h2>
            </header>
            <p>Si mi perfil es de tu interés, tienes alguna pregunta o te gustaría colaborar en un proyecto, no dudes en contactarme. Estoy abierto a nuevas oportunidades y conexiones.</p>
            <ul class="actions">
                <li><a href="mailto:{{ site.email }}" class="button next">Enviar un email</a></li>
            </ul>
        </div>
    </section>

</div>