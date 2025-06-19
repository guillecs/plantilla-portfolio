---
title: Mis Posts
subtitle: Reflexiones, tutoriales y artículos sobre mis intereses.
layout: page # Usa el layout de página estándar del tema Forty
permalink: /posts/ # La URL para ver todos los posts
---

<div id="main">
    <section id="one" class="tiles">
        {% for post in site.posts %}
            <article>
                <span class="image">
                    <img src="{{ site.baseurl }}/{{ post.image | default: 'assets/images/pic06.jpg' }}" alt="{{ post.alt | default: post.title }}" />
                </span>
                <header class="major">
                    <h3><a href="{{ post.url | relative_url }}" class="link">{{ post.title }}</a></h3>
                    <p>{{ post.subtitle | default: post.excerpt | strip_html | truncatewords: 20 }}</p>
                </header>
                <a href="{{ post.url | relative_url }}" class="link primary"></a>
            </article>
        {% endfor %}
    </section>
</div>