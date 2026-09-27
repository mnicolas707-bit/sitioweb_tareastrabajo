# Órdenes y Avisos

Aplicación web estática para registrar tareas, números de OT y avisos. No usa Flask, CDN, fuentes externas ni otros servicios: los datos se guardan en el almacenamiento local del navegador.

## Publicar en GitHub Pages

El workflow de GitHub Actions publica el sitio automáticamente al subir cambios a `main`. La aplicación estará disponible en <https://mnicolas707-bit.github.io/sitioweb_tareastrabajo/>. Para la primera publicación, habilitá GitHub Pages en **Settings → Pages** y seleccioná **GitHub Actions** como origen de publicación.

La página necesita abrirse al menos una vez con conexión para que el navegador descargue y guarde la aplicación para uso sin conexión. Después de esa primera visita, se puede abrir desde el mismo navegador incluso sin internet.

## Vista previa local

Con Python 3 instalado, ejecutá desde esta carpeta:

```text
python -m http.server 8000
```

Luego abrí `http://127.0.0.1:8000/` en el navegador. La caché sin conexión requiere servir la página por `localhost` o HTTPS.

## Copias de seguridad

Las tareas no se sincronizan con GitHub ni con otros equipos. Usá **Exportar copia** para guardar un archivo JSON y **Importar copia** para restaurarlo en este u otro navegador. Importar reemplaza las tareas actuales.
