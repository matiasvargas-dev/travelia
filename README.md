# ProyectoTp1 - Travelia

- `El diseño visual` está basado en esta paleta de colores y tipografía, incluida en `assets\img\Travelia branding presentation.png`.

Sitio web básico en HTML, CSS y contenido estático con varias vistas. Este proyecto está pensado como una página de agencia de viajes simple y completa.

## Estructura del proyecto

- `index.html` - Página principal del sitio.
- `views/` - Vistas secundarias que usan el mismo encabezado y pie de página.
  - `destinos.html`
  - `agencias.html`
  - `contactos.html`
  - `precios.html`
  - `blog.html`
- `includes/` - Componentes reutilizables cargados con JavaScript.
  - `header.html`
  - `footer.html`
- `styles/` - Estilos del proyecto.
  - `styles.css`
- `assets/` - Imágenes y otros recursos estáticos.
  - `img/`
  - `videos/`

## Cómo funciona el proyecto

- Cada página HTML tiene `<!DOCTYPE html>` al principio para usar HTML5.
- El archivo `styles/styles.css` define colores, tipografías y el diseño para todas las páginas.
- `includes/header.html` y `includes/footer.html` se cargan dentro de cada vista con `fetch()` desde JavaScript.
- Las rutas internas usan enlaces relativos dependiendo de la ubicación del archivo.

## Componentes principales

- `header.html`: Contiene el logo y el menú de navegación.
- `footer.html`: Contiene la información del pie de página y enlaces sociales.
- `styles.css`: Controla el estilo global, la estructura de tarjetas, el diseño responsivo y los efectos básicos.

## Uso local

1. Abre el proyecto en VS Code.
2. Abre `index.html` o cualquier archivo en `views/`.
3. Usa Live Server o abre el archivo en el navegador.

> Para ver los archivos `views/` correctamente, es mejor usar Live Server o un servidor local, porque las rutas relativas y las cargas de `fetch()` funcionan mejor desde HTTP.

## Documentación técnica

- El proyecto usa HTML5 en todas las páginas con etiquetas semánticas como `header`, `main`, `section`, `article` y `footer`.
- El archivo `styles/styles.css` centraliza todos los estilos; hay variables CSS definidas en `:root` para colores y tipografía.
- Se usan efectos con CSS puro: transiciones, transformaciones, filtros, layout con grid y flexbox, y un menú responsive para móvil.
- El contenido común del sitio se reutiliza cargando `includes/header.html` y `includes/footer.html` con JavaScript (`fetch()`), lo que facilita mantener el header y footer en un solo lugar.
- Las páginas del sitio son estáticas, por lo que no hay backend ni base de datos; todo se renderiza directamente en el navegador.

## Publicación del demo

Para entregar el proyecto es mejor subirlo a un repositorio remoto y publicar una versión en línea. Esto funciona igual que local, pero permite que cualquier persona vea el sitio desde internet.

### Opción 1: GitHub Pages

1. Sube todo el proyecto a un repositorio de GitHub.
2. En el repositorio, ve a `Settings` > `Pages`.
3. Selecciona la rama `main` o `master` y la carpeta `/root`.
4. Activa GitHub Pages y espera unos segundos.
5. Tu sitio quedará disponible en una URL tipo `https://usuario.github.io/nombre-repo/`.

### Opción 2: Netlify

1. Crea una cuenta en Netlify.
2. Conecta el repositorio de GitHub.
3. Elige la rama `main` o `master`.
4. Netlify publica el sitio automáticamente.

## Diferencia entre local y en línea

- Local: el sitio se ve en tu PC con Live Server o abriendo archivos desde VS Code.
- En línea: el sitio se sirve desde internet y cualquiera puede acceder con un enlace.
- La estructura y el código son los mismos; solo cambia dónde se carga el proyecto.

## Notas

- `index.html` es la página principal.
- Las páginas en `views/` están pensadas como secciones secundarias del mismo sitio.
- El proyecto es estático y no requiere backend.
- Si haces cambios en HTML o CSS, guarda los archivos y recarga el navegador.
