# Portfolio profesional — Pilar Ramírez

Portfolio en formato curso: página de inicio con tarjetas de sección, índice lateral desplegable y páginas cortas con navegación Anterior / Siguiente.

## Estructura

```
index.html        → la página completa (HTML + CSS + JS en un solo archivo)
img/retrato.webp  → retrato ilustrado (avatar)
img/*.webp        → capturas de los proyectos
```

## Publicar en GitHub Pages

1. Sube estos archivos al repositorio manteniendo la carpeta `img/`.
2. Ve a **Settings → Pages → Source**, elige la rama `main` y la carpeta raíz (`/`).
3. En un par de minutos estará en `https://tu-usuario.github.io/nombre-del-repo/`.

## Formulario de contacto

Usa Web3Forms con la misma clave que el portfolio creativo (constante `WEB3FORMS_ACCESS_KEY` en `index.html`). Los mensajes llegan al correo asociado a esa clave. No hace falta configurar nada más.

## Añadir capturas a un proyecto

1. Guarda las imágenes en `img/` (por ejemplo `udl_1.webp`).
2. En `index.html`, busca el proyecto dentro de `const PROJECTS` y añade:
   ```js
   "images": [["udl_1.webp", "Descripción de la captura"], ["udl_2.webp", "Otra descripción"]],
   ```

## Vista previa al compartir el enlace

Cuando sepas la URL final, cambia en `index.html` la ruta de `og:image` por la dirección completa, por ejemplo `https://tu-usuario.github.io/nombre-del-repo/img/retrato.webp`, para que LinkedIn y WhatsApp muestren tu retrato.
