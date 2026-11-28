# Notion: From Zero to Hero

Repositorio de referencia de la charla/taller: diapositivas, guion del ponente y material para seguir practicando después de la sesión.

La sesión está pensada para **45 minutos + 15 minutos de preguntas**. Las diapositivas se editan con [Slidev](https://sli.dev/).

## Material del taller

- [Diapositivas y guion](slides.md): las notas del ponente están en comentarios HTML junto a cada diapositiva; también se ven en el modo presentador.
- **Versión web prevista:** <https://CrisKrus.github.io/notion-from-zero-to-hero-talk/> (disponible cuando se active Pages y se complete el primer despliegue).
- **Ejercicios:** están en una página de Notion, pendiente de enlazar e incorporar a este repositorio. Las diapositivas también incluyen propuestas para practicar.

Al incorporar más contenido, usar `ejercicios/` para enunciados y soluciones, `material/` para recursos complementarios y `public/` para archivos que deban acompañar a la web, como imágenes o un PDF descargable. Estas carpetas se crearán cuando haya contenido real. Si el guion crece, se puede separar en `guion.md`.

## Ejecutar y presentar

Requisitos: **Node.js 24 o superior** y **pnpm 11.5.1** (versión fijada en `package.json`).

```bash
git clone git@github.com:CrisKrus/notion-from-zero-to-hero-talk.git
cd notion-from-zero-to-hero-talk
pnpm install --frozen-lockfile
pnpm dev
```

Slidev abre el navegador. El modo presentador permite consultar las notas y el tiempo de la sesión.

## Generar HTML y PDF

```bash
pnpm build        # Web estática en dist/, para servir desde la raíz
pnpm build:pages  # Web en dist/, con la ruta del repositorio y navegación hash
pnpm export       # Exportación PDF de Slidev (requiere playwright-chromium)
```

La exportación PDF es opcional y no forma parte del despliegue automático. Si Slidev solicita `playwright-chromium`, hay que instalarlo con `pnpm add -D playwright-chromium` y preparar su navegador siguiendo la [guía de exportación](https://sli.dev/guide/exporting).

El PDF local por defecto (`slides.pdf`) se ignora. Para distribuir una versión revisada, se puede guardar expresamente en `public/`; Slidev la copiará a la web al compilar. No se ignoran todos los PDF, ya que también pueden ser material del taller.

## Publicar en GitHub Pages

1. En GitHub, abrir **Settings → Pages → Build and deployment → Source → GitHub Actions**.
2. Subir los cambios a `main`.
3. Comprobar que termina correctamente el workflow **Publicar diapositivas en GitHub Pages**.

El workflow `.github/workflows/deploy-pages.yml` instala las dependencias con el lockfile, genera el HTML y publica `dist/` como artefacto de Pages. No hace falta guardar el HTML generado en Git. También puede ejecutarse manualmente desde Actions una vez subido.

La ruta de publicación usa el nombre del remoto: `notion-from-zero-to-hero-talk`. Si cambia ese nombre, actualizar `build:pages` y los enlaces de este README.

Las notas del ponente se incluyen en la versión web y en el código fuente público: no deben contener información privada. Configuración basada en la [guía de alojamiento de Slidev](https://sli.dev/guide/hosting).

## Preparación de la charla

Preparar en Notion una página de pruebas y las bases `Tareas` y `Proyectos`, con registros ficticios. Ensayar las cinco demostraciones (3 + 2 + 6 + 4 + 5 minutos). La disponibilidad de funciones como gráficos y automatizaciones puede variar según el plan y los permisos.

Antes de compartir el material, revisar capturas, enlaces y datos para evitar publicar información personal, credenciales o contenido privado del workspace.

## Qué se versiona

Se conservan las fuentes, el guion, los ejercicios, los recursos, `package.json` y `pnpm-lock.yaml`. Se excluyen dependencias (`node_modules/`), compilaciones (`dist/`), cachés, archivos de macOS (`.DS_Store`), logs y configuración local con posibles secretos (`.env*`, excepto plantillas `.example`).
