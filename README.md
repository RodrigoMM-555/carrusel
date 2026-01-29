# jocarsacarrusel

Una librería ligera y sencilla para implementar un carrusel de imágenes dinámico en sitios web, optimizada para GitHub Pages.
Características

    Generación dinámica: Organiza automáticamente las imágenes dentro de una sección interna.

    Controles integrados: Crea botones de navegación (anterior/siguiente) automáticamente.

    Transiciones fluidas: Animaciones suaves mediante CSS transition.

    Dimensiones estándar: Configurado para una resolución de 1280px x 720px.

Instalación

Solo necesitas incluir los archivos CSS y JS en tu proyecto:
HTML

<link rel="stylesheet" href="jocarsacarrusel.css">
<script src="jocarsacarrusel.js" defer></script>

Uso

Para implementar el carrusel, estructura tu HTML de la siguiente manera:
HTML

<div class="jocarsacarrusel">
    <img src="imagen1.jpg" alt="Descripción 1">
    <img src="imagen2.jpg" alt="Descripción 2">
    <img src="imagen3.jpg" alt="Descripción 3">
</div>

El script se encargará de:

    Extraer las imágenes.

    Envolverlas en un contenedor section.

    Añadir la funcionalidad de los botones de navegación.

Estructura Técnica

    Viewport: El contenedor principal tiene un ancho fijo y overflow: hidden.

    Desplazamiento: La navegación funciona modificando la propiedad left del contenedor interno basado en un índice (contador) multiplicado por el ancho de la imagen (1280px).
