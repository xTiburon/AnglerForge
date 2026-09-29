# Angler Forge — sitio web

Sitio estático. No necesita compilación ni servidor especial.

## Estructura

```
index.html                     Página completa (estilos, fuentes, iconos y logo incluidos)
assets/portfolio/minecraft/    Portafolio · Plugins de Minecraft (capturas)
assets/portfolio/discord/      Portafolio · Bots de Discord (capturas)
assets/portfolio/diseno/       Portafolio · Ilustraciones, chibis, banners, logotipos y mascotas
assets/portfolio/web/          Portafolio · Páginas web (capturas)
  └─ thumbs/                   Miniaturas ligeras para la cuadrícula (la imagen grande se usa al ampliar)
assets/brand/                  Logo y mascotas en archivo (copia de respaldo)
```

`index.html` carga las imágenes de `assets/portfolio/` por ruta relativa: mantén la carpeta `assets/` junto a `index.html`.

Las carpetas `assets/gd/` y `assets/pf/` ya no se usan y se pueden borrar.

## Añadir un trabajo al portafolio

1. Copia la imagen en la carpeta de su categoría dentro de `assets/portfolio/` (y, si es grande, una versión reducida de unos 700 px en `thumbs/`).
2. Añade una línea a la lista `ITEMS` de la página con su `id`, categoría (`mc`, `dc`, `gd`, `wb`), tipo, ruta, tamaño en píxeles y título en español e inglés. Esa lista está dentro de la plantilla empaquetada (codificada como JSON) de `index.html`, así que conviene editarla con una herramienta y no a mano.

## Publicar con GitHub Pages

1. Sube todo el contenido de esta carpeta a la raíz del repositorio.
2. En el repo: **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)`. Guarda.
4. En uno o dos minutos el sitio queda en `https://<usuario>.github.io/<repo>/`.

También funciona en Netlify, Vercel o cualquier hosting: sube la carpeta tal cual.
