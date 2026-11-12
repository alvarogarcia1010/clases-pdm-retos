# Clases · Desarrollo Móvil · Instituto Retos

Decks, talleres y guías del módulo Desarrollo Móvil (React Native). Se publica con GitHub Pages.

## Estructura

```
index.html              Portada: lista de ciclos
assets/deck.css         Guía de estilo de los decks (Reveal.js)
assets/site.css         Estilo de las páginas índice
_plantilla/index.html   Esqueleto para arrancar una clase nueva
guias/
  index.html            Lista de guías (sirven en cualquier ciclo)
  01-instalacion/       Una carpeta por guía: NN-nombre-corto/index.html
ciclo-03-2026/
  index.html            Índice del ciclo: una tarjeta por sesión (es el enlace que reciben los estudiantes)
  01-introduccion/      Una carpeta por sesión: NN-nombre-corto/index.html
  02-.../
```

## Para agregar una clase

1. Copiá `_plantilla/` a `ciclo-XX-AAAA/NN-nombre-corto/`.
2. Editá el deck. Reglas de estilo: Reveal.js 5.1.0 a 1280x720, Prism para código (nunca highlight.js), una idea clave por slide, sin em dashes, todo debe caber sin scroll.
3. En `ciclo-XX-AAAA/index.html`, convertí la tarjeta de la sesión en enlace (`<a class="sesion ..." href="NN-nombre-corto/">`) y quitale la clase `pendiente`.
4. Commit y push. Pages lo publica en un par de minutos.

## Para agregar una guía

1. Creá `guias/NN-nombre-corto/index.html` (usá `guias/01-instalacion/index.html` de base: enlaza `../../assets/site.css` y usa las clases `.guide`, `.steps`, `.check`, `.err`).
2. Agregá su tarjeta en `guias/index.html`.

## Qué no va aquí

El repo es público. Rúbricas con criterios de calificación, listas de estudiantes, notas y archivos del LMS se quedan fuera.

## Publicación

Settings → Pages → Deploy from a branch → `main` / `(root)`. El archivo `.nojekyll` hace que Pages sirva también la carpeta `_plantilla`.
