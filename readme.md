[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/fIoohYgs)
# Lab 2 — Catálogo de Películas y Series 🎬

Crea un mini-sitio web que catalogue películas y series. Practicarás HTML semántico, navegación entre páginas y el uso de elementos multimedia.

Última actualización: 5 de noviembre de 2025

## Objetivos de aprendizaje

- Estructurar un sitio web con HTML5 semántico utilizando las etiquetas:
  - `<header>` → Para encabezados de página
  - `<nav>` → Para menús de navegación
  - `<body>` → Estructura principal del documento
  - `<section>` → Para dividir el contenido en secciones
  - `<footer>` → Para pie de página
- Crear contenido utilizando:
  - `<p>` → Para párrafos descriptivos
  - `<ul>` y `<li>` → Para listas de características o elementos no ordenados
  - `<ol>` y `<li>` → Para rankings o listas ordenadas
- Implementar elementos multimedia:
  - `<video>` → Para incluir tráilers
  - `<audio>` → Para bandas sonoras o efectos
- Crear navegación funcional entre las tres páginas del sitio

## Requisitos previos

- Conocer etiquetas HTML básicas y rutas relativas.
- Tener un editor (VS Code) y un navegador.

## Qué vas a construir (resumen)

Un sitio web de 3 páginas interconectadas:
- `index.html`: Página de bienvenida con navegación a las secciones de películas y series
- `movies.html`: Catálogo de películas con listas, tráilers y contenido multimedia
- `series.html`: Catálogo de series con listas, tráilers y contenido multimedia

## Estructura del proyecto

```
lab2-catalogo/
├─ index.html                # Página de bienvenida y navegación principal
├─ movies.html              # Catálogo de películas
├─ series.html             # Catálogo de series
└─ assets/
   ├─ images/              # Imágenes y posters
   ├─ video/              # Tráilers de películas y series
   └─ audio/              # Bandas sonoras y efectos
```

## Reglas técnicas obligatorias

1. Estructura HTML5 semántica en cada página:
   - `<header>` para la cabecera
   - `<nav>` para el menú de navegación
   - `<body>` correctamente estructurado
   - `<section>` para dividir el contenido
   - `<footer>` para el pie de página

2. En `index.html`:
   - Título de bienvenida
   - Navegación clara a movies.html y series.html
   - Al menos un párrafo `<p>` descriptivo
   - Lista `<ul>` con características del catálogo

3. Requisitos de contenido mínimo:

   En `movies.html`:
   - Incluir al menos 4 películas diferentes
   - Cada película debe tener:
     * Portada (usando `<img>`)
     * Tráiler (usando `<video>`)
     * Banda sonora (usando `<audio>`)
   - Usar `<ul>` para listar características de cada película
   - Usar `<ol>` para crear un ranking de las películas
   - Párrafos `<p>` con sinopsis de cada película

   En `series.html`:
   - Incluir al menos 4 series diferentes
   - Cada serie debe tener:
     * Portada (usando `<img>`)
     * Tráiler (usando `<video>`)
     * Banda sonora o tema principal (usando `<audio>`)
   - Usar `<ul>` para listar características de cada serie
   - Usar `<ol>` para ranking o temporadas
   - Párrafos `<p>` con sinopsis de cada serie

4. Requisitos generales:
   - Enlaces funcionales entre todas las páginas
   - Rutas relativas correctas
   - Elementos multimedia con controles
   - Textos alternativos en imágenes
   - Organización clara del contenido

> Nota sobre contenidos: utiliza recursos con permiso/licencia adecuada (propios, dominio público o libres de derechos). Si incrustas contenido de terceros (por ejemplo, un tráiler en una plataforma oficial), respeta sus políticas de uso.

## Pasos sugeridos (guía)

1. Configura la estructura del proyecto:
   - Crea las carpetas necesarias
   - Inicializa los tres archivos HTML

2. Desarrolla `index.html`:
   - Estructura básica con header, nav, body y footer
   - Título de bienvenida al catálogo
   - Menú de navegación a las otras páginas
   - Lista de características del sitio
   - Párrafo introductorio

3. Crea `movies.html`:
   - Mantén la estructura semántica HTML5
   - Agrega una lista ordenada de películas destacadas
   - Incluye tráilers usando `<video>`
   - Añade descripción con párrafos
   - Incorpora audio relacionado

4. Desarrolla `series.html`:
   - Sigue la misma estructura semántica
   - Crea listas no ordenadas de series por género
   - Agrega tráilers relevantes
   - Incluye descripciones detalladas
   - Añade elementos de audio

5. Para todas las páginas:
   - Verifica la navegación entre páginas
   - Comprueba que los elementos multimedia funcionen
   - Revisa los textos alternativos
   - Asegura que las rutas sean correctas

## Ejemplos de código

### Ejemplo de entrada de película/serie

```html
<section>
    <h2>Nombre de la Película/Serie</h2>
    
    <!-- Portada -->
    <img src="assets/images/portada.jpg" alt="Portada de [Título]">
    
    <!-- Sinopsis -->
    <p>
        Descripción o sinopsis de la película/serie...
    </p>
    
    <!-- Características -->
    <ul>
        <li>Director: [Nombre]</li>
        <li>Año: [YYYY]</li>
        <li>Género: [Género]</li>
        <li>Duración: [XXX min]</li>
    </ul>
    
    <!-- Tráiler -->
    <h3>Tráiler</h3>
    <video controls width="100%">
        <source src="assets/video/trailer.mp4" type="video/mp4">
        Tu navegador no soporta el elemento video.
    </video>
    
    <!-- Banda Sonora -->
    <h3>Tema Principal</h3>
    <audio controls>
        <source src="assets/audio/theme.mp3" type="audio/mpeg">
        Tu navegador no soporta el elemento audio.
    </audio>
</section>
```

### Estructura básica (todas las páginas)

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Catálogo de Películas y Series</title>
</head>
<body>
    <header>
        <h1>Título de la página</h1>
        <nav>
            <ul>
                <li><a href="index.html">Inicio</a></li>
                <li><a href="movies.html">Películas</a></li>
                <li><a href="series.html">Series</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section>
            <!-- Contenido específico de cada página -->
        </section>
    </main>

    <footer>
        <p>Creado por [Tu Nombre] - 2025</p>
    </footer>
</body>
</html>
```

### Listas (para movies.html y series.html)

```html
<!-- Lista no ordenada de géneros (ul) -->
<section>
    <h2>Géneros disponibles</h2>
    <ul>
        <li>Acción y Aventura</li>
        <li>Comedia</li>
        <li>Drama</li>
        <li>Ciencia Ficción</li>
    </ul>
</section>

<!-- Lista ordenada de más vistos (ol) -->
<section>
    <h2>Top 5 más populares</h2>
    <ol>
        <li>Título 1 (2023) - ★★★★★</li>
        <li>Título 2 (2024) - ★★★★☆</li>
        <li>Título 3 (2023) - ★★★★☆</li>
        <li>Título 4 (2024) - ★★★★☆</li>
        <li>Título 5 (2023) - ★★★★☆</li>
    </ol>
</section>
```

### Video (tráiler)

```html
<section>
  <h2>Tráiler oficial</h2>
  <video controls preload="metadata" poster="assets/images/poster.jpg" width="100%">
    <source src="assets/video/trailer.mp4" type="video/mp4">
    <source src="assets/video/trailer.webm" type="video/webm">
    <!-- Subtítulos opcionales si cuentas con un archivo VTT -->
    <!-- <track kind="subtitles" src="assets/video/subtitulos.vtt" srclang="es" label="Español"> -->
    Tu navegador no soporta el elemento video.
  </video>
</section>
```

Si vas a incrustar desde una plataforma (p. ej., reproductor oficial), usa su código de inserción permitido y asegúrate de que sea legal/permitido.

### Audio (tema principal)

```html
<section>
  <h2>Tema principal</h2>
  <audio controls preload="none">
    <source src="assets/audio/theme.mp3" type="audio/mpeg">
    <source src="assets/audio/theme.ogg" type="audio/ogg">
    Tu navegador no soporta el elemento audio.
  </audio>
</section>
```

## Buenas prácticas y accesibilidad

- Usa `lang="es"` en `<html>` y `meta charset="utf-8"`, `meta name="viewport"` en `<head>`.
- Títulos jerárquicos (`h1` una vez por página, luego `h2`, `h3`…).
- Descripciones y textos de enlace claros (evita "haz clic aquí").
- Imágenes con `alt` significativo.
- Video/audio con `controls` y, si es posible, subtítulos/transcripción.
- Navegación consistente en las 3 páginas.

## Entregables

1. Repositorio en GitHub que contenga:
   - `index.html`, `movies.html`, `series.html`
   - Carpeta `assets/` con todas las imágenes, videos y audios utilizados
   - Un archivo README.md que incluya:
     * Título del proyecto
     * Lista de películas incluidas
     * Lista de series incluidas
     * Fuentes de los recursos multimedia utilizados
     * URL del sitio publicado en GitHub Pages

2. Publicación en GitHub Pages:
   - Ir a Settings > Pages en el repositorio
   - En "Source", seleccionar "main" como branch
   - Guardar y esperar a que el sitio se publique
   - Incluir la URL del sitio publicado en el README.md

> Nota: Asegúrate de que todas las rutas en tu código HTML sean relativas para que funcionen correctamente en GitHub Pages.

## Rúbrica de evaluación (100 pts)

- Estructura HTML5 semántica (20 pts):
  - Uso correcto de `<header>`: 5 pts
  - Implementación de `<nav>`: 5 pts
  - Estructura de `<section>`: 5 pts
  - Uso apropiado de `<footer>`: 5 pts

- Contenido y listas (30 pts):
  - Párrafos `<p>` informativos: 10 pts
  - Listas no ordenadas `<ul>`: 10 pts
  - Listas ordenadas `<ol>`: 10 pts

- Elementos multimedia (30 pts):
  - Videos con controles: 15 pts
  - Audio con controles: 15 pts

- Navegación y publicación (20 pts):
  - Enlaces funcionales entre páginas: 5 pts
  - Organización de archivos y recursos: 5 pts
  - Repositorio en GitHub: 5 pts
  - Sitio publicado correctamente en GitHub Pages: 5 pts

## Checklist de validación rápida

Estructura básica:
- [ ] Las tres páginas están creadas (index.html, movies.html, series.html)
- [ ] La navegación funciona correctamente entre todas las páginas
- [ ] Cada página usa correctamente las etiquetas semánticas (header, nav, section, footer)
- [ ] El proyecto está subido a GitHub
- [ ] El sitio está publicado y accesible en GitHub Pages

Para movies.html:
- [ ] Contiene al menos 4 películas diferentes
- [ ] Cada película tiene portada (img), tráiler (video) y banda sonora (audio)
- [ ] Incluye listas ordenadas y no ordenadas
- [ ] Los párrafos describen cada película

Para series.html:
- [ ] Contiene al menos 4 series diferentes
- [ ] Cada serie tiene portada (img), tráiler (video) y tema principal (audio)
- [ ] Incluye listas ordenadas y no ordenadas
- [ ] Los párrafos describen cada serie

Aspectos técnicos:
- [ ] Todas las imágenes tienen textos alternativos
- [ ] Todos los videos y audios tienen controles
- [ ] Las rutas relativas funcionan correctamente
- [ ] El código está correctamente indentado y organizado

## Recursos útiles

- MDN Web Docs: HTML — https://developer.mozilla.org/es/docs/Web/HTML
- `<video>` — https://developer.mozilla.org/es/docs/Web/HTML/Element/video
- `<audio>` — https://developer.mozilla.org/es/docs/Web/HTML/Element/audio
- Listas (`<ul>`, `<ol>`) — https://developer.mozilla.org/es/docs/Web/HTML/Element/ul y https://developer.mozilla.org/es/docs/Web/HTML/Element/ol
- Subtítulos VTT — https://developer.mozilla.org/es/docs/Web/API/WebVTT_API
- Medios libres de derechos: 
  - Pexels (video): https://www.pexels.com/es-es/videos/
  - Pixabay (audio): https://pixabay.com/es/music/

## Datos del docente

- Pablo Pérez Martínez
    - paperez@puce.edu.ec
    - pablo.perez@uisek.edu.ec
