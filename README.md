# Control VP (Cuadraditos)

PWA en un solo archivo (`index.html`). Los datos quedan guardados en cada navegador (localStorage); no se suben a GitHub.

## Publicar en GitHub Pages (una sola vez)
1. Creá un repositorio nuevo en GitHub (por ejemplo `control-vp`).
2. Subí **todo el contenido de esta carpeta** a la raíz del repo (Add file → Upload files), incluido `.nojekyll`.
3. Settings → Pages → Source: *Deploy from a branch* → Branch `main` / carpeta `/ (root)` → Save.
4. A los 1–2 minutos queda en `https://TU-USUARIO.github.io/control-vp/`. Abrilo y usá "Instalar app" desde el navegador.

## Actualizar
1. Reemplazá `index.html` en el repo por la versión nueva.
2. Subí el número de versión en **dos lugares** (mismo número, ej. `2026101301`):
   - `index.html` → `sw-tablero.js?v=...`
   - `sw-tablero.js` → `CACHE_VERSION = 'controlvp-...'`
3. Commit. La app instalada toma la versión nueva al reabrirla (a veces hace falta cerrarla y abrirla dos veces).

## Ojo con los datos
Cambiar de dirección (de la PC/localhost a github.io) implica otro "origen": los datos guardados en la versión vieja **no pasan solos**. Exportá un respaldo desde la versión vieja e importalo en la nueva antes de dejar de usarla.
