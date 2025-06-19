---
title: Mis Proyectos
subtitle: Descubre mi trabajo más reciente y mis estudios de caso.
layout: page # Usa el layout de página estándar del tema Forty
permalink: /proyectos/ # Asegura que la URL sea /proyectos/
---

<div id="main">
    <section id="one" class="tiles">
        {% for project in site.projects %}
            <article>
                <span class="image">
                    <img src="{{ site.baseurl }}/{{ project.image }}" alt="{{ project.alt }}" />
                </span>
                <header class="major">
                    <h3><a href="{{ project.url | relative_url }}" class="link">{{ project.title }}</a></h3>
                    <p>{{ project.subtitle }}</p>
                </header>
                <a href="{{ project.url | relative_url }}" class="link primary"></a>
            </article>
        {% endfor %}
    </section>
</div>