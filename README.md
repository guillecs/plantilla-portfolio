# Mi Portfolio Simple - Jekyll Theme

Una versión simplificada y personalizable del tema "Forty" de [HTML5 UP](https://html5up.net/), adaptado para un portfolio digital fácil de usar y mantener con Jekyll.

![Forty Theme](assets/images/forty.jpg "Forty Theme")

## Cómo Usar Esta Plantilla

Esta plantilla está diseñada para ser minimalista y fácil de actualizar. Sigue estos pasos para personalizarla:

### 1. Configuración Inicial (`_config.yml`)

Abre el archivo `_config.yml` en la raíz de tu proyecto y actualiza lo siguiente:

* **`title` y `subtitle`**: Tu nombre y una frase corta para tu portfolio.
* **`email`**: Tu dirección de correo electrónico para el botón de contacto en el CV y la página "Sobre Mí".
* **`socials`**: Añade tus perfiles de redes sociales (ej. GitHub, LinkedIn). Solo se mostrarán los que incluyas.
* **`tiles`**: **¡Importante para el orden!** Define aquí los "cuadritos" que aparecerán en tu página principal (`Home`). El orden en esta lista será el orden en que se muestran.

    ```yaml
    # Ejemplo de la sección 'tiles' en _config.yml
    tiles:
      - title: Sobre Mí
        subtitle: Mi Experiencia y Pasiones
        image: assets/images/pic07.jpg
        url: /sobre-mi/
      - title: Proyectos
        subtitle: Mis trabajos integrales y estudios de caso
        image: assets/images/pic01.jpg
        url: /proyectos/
      # ... y así sucesivamente para Posts, CV, etc.
    ```

### 2. Actualizar tu Página "Sobre Mí"

* Abre el archivo **`sobre-mi.md`** en la raíz de tu proyecto.
* Edita el **"Front Matter"** (la información entre los `---`) con tu título, subtítulo e imagen principal.
* Modifica el contenido HTML y Markdown en el cuerpo para presentar tu perfil profesional.

### 3. Gestionar tus Proyectos

* Tus proyectos se encuentran en la carpeta **`_projects/`**.
* Para añadir un nuevo proyecto, crea un nuevo archivo `.md` dentro de `_projects/` (ej., `mi-nuevo-proyecto.md`).
* **Estructura de un archivo de proyecto:**
    * **Front Matter:**
        ```yaml
        ---
        title: El Título de tu Proyecto
        subtitle: Una descripción corta para el cuadrito.
        image: assets/images/imagen-proyecto.jpg # Ruta de la imagen para el cuadrito y la cabecera.
        alt: Descripción de la imagen.
        date: YYYY-MM-DD HH:MM:SS +/-HHMM # Fecha de creación.
        layout: project # O 'page', según tu configuración.
        ---
        ```
    * **Contenido (Markdown + HTML):** Usa Markdown para texto, encabezados, listas. Para imágenes dentro del contenido, usa:
        ```html
        <span class="image main">
            <img src="{{ site.baseurl }}/assets/images/tu-imagen-interna.jpg" alt="Descripción de la imagen" />
            <figcaption>Pie de foto (opcional).</figcaption>
        </span>
        ```
* **Guía de Ejemplo:** Consulta `_projects/guia-para-nuevos-proyectos.md` para ver un ejemplo detallado de cómo estructurar un proyecto.

### 4. Gestionar tus Posts (Artículos/Blog)

* Tus posts se encuentran en la carpeta **`_posts/`**.
* Para añadir un nuevo post, crea un nuevo archivo `.md` con este formato de nombre: `YYYY-MM-DD-titulo-del-post.md` (ej., `2024-06-20-mi-primer-articulo.md`).
* **Estructura de un archivo de post:**
    * **Front Matter:**
        ```yaml
        ---
        layout: post
        title: El Título de tu Post
        subtitle: Un resumen corto para la lista de posts.
        image: assets/images/imagen-post.jpg # Imagen para el cuadrito del post.
        alt: Descripción de la imagen.
        date: YYYY-MM-DD HH:MM:SS +/-HHMM # Fecha de publicación.
        categories: [Categoría1, Categoría2] # Opcional.
        tags: [tag1, tag2] # Opcional.
        ---
        ```
    * **Contenido (Markdown):** Escribe el cuerpo de tu artículo usando Markdown.
* **Guía de Ejemplo:** Consulta `_posts/2024-06-20-como-crear-un-post.md` para un ejemplo práctico.

### 5. Actualizar tu CV

* Abre el archivo **`cv.md`** en la raíz de tu proyecto.
* **Para añadir tu CV en PDF:**
    1.  Guarda tu archivo PDF de CV dentro de `assets/cv/`.
    2.  En `cv.md`, actualiza el enlace del botón de descarga:
        ```html
        <li><a href="{{ site.baseurl }}/assets/cv/tu-cv-nombre.pdf" class="button next icon solid fa-download">Descargar CV en PDF</a></li>
        ```
        Asegúrate de que `tu-cv-nombre.pdf` coincide con el nombre real de tu archivo.
* Puedes modificar el texto introductorio en `cv.md` para que se adapte a tu estilo.

### 6. Cómo Añadir Imágenes

* Todas las imágenes de tu portfolio deben ir en la carpeta **`assets/images/`**.
* **Para imágenes en el Front Matter (tiles, banners):**
    ```yaml
    image: assets/images/mi-imagen-hero.jpg
    alt: Descripción de la imagen
    ```
* **Para imágenes dentro del contenido (proyectos, posts, páginas):**
    ```html
    <span class="image main">
        <img src="{{ site.baseurl }}/assets/images/mi-imagen-contenido.jpg" alt="Descripción de la imagen" />
        <figcaption>Pie de foto (opcional).</figcaption>
    </span>
    ```



