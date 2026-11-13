# Design Styles and Movements · ID4A

Sitio web para que los estudiantes de ID4A (POLI.design) exploren el contenido de *Design Styles and Movements — Past references*.
Contenido: Silvia Ferraris · Slides y sitio: Martina Labarta · 2026.

## Publicar en GitHub Pages
1. Crea un repositorio nuevo en GitHub (p. ej. `id4a-design-styles`).
2. Sube **todo el contenido de esta carpeta** a la raíz del repositorio (Add file → Upload files: arrastra `index.html`, `content.js`, `.nojekyll`, `README.md` y las carpetas `img/` y `tools/`).
3. Ve a **Settings → Pages**, en *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. En 1–2 minutos el sitio estará en `https://<tu-usuario>.github.io/id4a-design-styles/`.

## Contraseña
- Todo el texto del sitio está cifrado dentro de `content.js`; solo se lee con la contraseña.
- Las imágenes de la carpeta `img/` no están cifradas. Si el repositorio es público, también son visibles en GitHub.

### Cambiar la contraseña
1. Abre `https://<tu-usuario>.github.io/id4a-design-styles/tools/password.html`.
2. Escribe la contraseña actual y la nueva → **Generar nuevo content.js** → descárgalo.
3. Sube ese `content.js` al repositorio sustituyendo el anterior y haz *Commit*.

La contraseña antigua deja de funcionar en cuanto se publica el nuevo archivo.

## Estructura
- `index.html` — el sitio (índice con imágenes al pasar el cursor, mapa interactivo y páginas por movimiento)
- `content.js` — contenido cifrado (AES-256-GCM, clave PBKDF2-SHA256)
- `img/` — imágenes, agrupadas en un archivo por movimiento
- `tools/password.html` — herramienta para cambiar la contraseña
