# Angler Forge — sitio web

Sitio estático. No necesita compilación ni servidor especial.

## Estructura

```
index.html          Página completa (estilos, fuentes, iconos y logo incluidos)
assets/gd/          Portafolio · Diseño gráfico
assets/pf/          Portafolio · Minecraft, Discord, Web y logotipos
assets/brand/       Logo y mascotas en archivo (copia de respaldo)
```

`index.html` carga las imágenes de `assets/gd/` y `assets/pf/` por ruta relativa: mantén la carpeta `assets/` junto a `index.html`.

## Publicar con GitHub Pages

1. Sube todo el contenido de esta carpeta a la raíz del repositorio.
2. En el repo: **Settings → Pages → Build and deployment → Deploy from a branch**.
3. Elige la rama `main` y la carpeta `/ (root)`. Guarda.
4. En uno o dos minutos el sitio queda en `https://<usuario>.github.io/<repo>/`.

También funciona en Netlify, Vercel o cualquier hosting: sube la carpeta tal cual.
