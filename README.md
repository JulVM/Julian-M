# Sitio web de Julian Valderrama

Landing page estática para presentar servicios de consultoría en gestión humana, analítica de datos y optimización de procesos.

## Contenido

- `index.html`: página, estilos y JavaScript.
- `assets/`: imágenes y logotipo utilizados por la página. Conserva los nombres en minúscula tal como aparecen para evitar errores de rutas en GitHub Pages.
- `.github/workflows/deploy-pages.yml`: publicación automática en GitHub Pages.

## Publicar en GitHub Pages

1. Sube `index.html`, `README.md`, la carpeta completa `assets/` y `.github/workflows/deploy-pages.yml` a la raíz de la rama `main`. GitHub distingue mayúsculas y minúsculas en los nombres y las rutas; no cambies los nombres de los archivos dentro de `assets/`.
2. En el repositorio, abre **Settings → Pages** y selecciona **GitHub Actions** como fuente de publicación.
3. Cada vez que se actualice la rama `main`, el flujo publicará la página. También puedes iniciarlo manualmente desde **Actions → Deploy to GitHub Pages → Run workflow**.
4. Al terminar la primera ejecución, encontrarás la URL pública en **Settings → Pages** o en el resumen de la ejecución del flujo.

No se requiere instalar dependencias ni compilar el sitio.

El flujo verifica que todas las imágenes y el favicon estén incluidos antes de publicar. Si Actions indica que falta un recurso, sube la carpeta `assets/` completa a la raíz del repositorio, al mismo nivel que `index.html`, y vuelve a ejecutar el despliegue.

## Antes de publicar

- Confirma que el nombre y las imágenes de `assets/` sean adecuados para compartir públicamente.
- Actualiza los enlaces de redes sociales si quieres dirigirlos a perfiles específicos.
- El formulario solo valida los campos y muestra una confirmación en el navegador; no transmite ni almacena mensajes. WhatsApp y Telegram están disponibles como alternativas directas.
- La tipografía Poppins se carga desde Google Fonts y requiere conexión a internet; se usa una tipografía de respaldo si el servicio no está disponible.
