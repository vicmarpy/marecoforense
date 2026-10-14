# marecoforense.com.py

Sitio estático hecho con [Hugo](https://gohugo.io). Gratis de alojar (Cloudflare Pages o GitHub Pages).

## 1. Instalar Hugo (versión "extended")

- Windows: `winget install Hugo.Hugo.Extended`
- macOS: `brew install hugo`
- Linux: descargar desde https://github.com/gohugoio/hugo/releases

Comprobar con `hugo version`.

## 2. Completar los datos de contacto

Abrir `hugo.toml` y completar `email`, `whatsapp` y `telefono` (en la sección `[params]`). Mientras estén vacíos, Hugo avisa con una advertencia y la página de contacto no muestra datos.

## 3. Ver el sitio en tu computadora

```
hugo server -D
```

Abrir http://localhost:1313. La opción `-D` muestra también los borradores.

## 4. Escribir una nota

```
hugo new notas/nombre-de-la-nota.md
```

Se crea `content/notas/nombre-de-la-nota.md` con la plantilla (resumen, contexto, procedimiento, hallazgos, recomendaciones, referencias). Al terminar, cambiar `draft: true` por `draft: false` (o borrar esa línea) para que se publique.

La nota `cadena-de-custodia-evidencia-digital.md` es un ejemplo en borrador: editarla, reemplazarla o borrarla.

## 5. Publicar

### Opción A: Cloudflare Pages (recomendada)

1. Subir esta carpeta a un repositorio de GitHub.
2. En Cloudflare: Workers & Pages → Create → Pages → Connect to Git.
3. Configuración de compilación:
   - Build command: `hugo --gc --minify`
   - Build output directory: `public`
   - Variable de entorno: `HUGO_VERSION` = `0.147.0`
4. En Custom domains, agregar `marecoforense.com.py` y seguir las instrucciones de DNS que indique Cloudflare.

### Opción B: GitHub Pages

1. Subir esta carpeta a un repositorio de GitHub (rama `main`).
2. En Settings → Pages → Source, elegir **GitHub Actions**. El archivo `.github/workflows/hugo.yml` ya está listo.
3. En Settings → Pages → Custom domain, escribir `marecoforense.com.py`.
4. En el panel DNS del dominio, crear los registros que indique GitHub (CNAME hacia `<usuario>.github.io`, o registros A para el dominio raíz).

## Estructura

```
hugo.toml            configuración y datos de contacto
archetypes/notas.md  plantilla de nota nueva
content/             páginas: inicio, perfil, servicios, contacto y notas/
layouts/             plantillas HTML del sitio
static/              CSS y favicon
```
