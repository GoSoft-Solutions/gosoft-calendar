# GoSoft Calendar

Landing page para agendar reuniones con el Team de GoSoft mediante **Google Calendar Appointment Scheduling**.

🌐 **Producción:** [calendar.gosoftsolutions.com](https://calendar.gosoftsolutions.com)

## Estructura

```
gosoft-calendar/
├── index.html           # Página principal con el botón de Google Calendar
├── 404.html             # Página de error con animación Lottie
├── 404-error.json       # Animación Lottie del 404
├── css/style.css        # Estilos (incluye ajustes al modal de Google)
├── images/
│   └── gosoft-logo.png  # Logo del header
├── favicon.ico
├── vercel.json          # Headers de seguridad HTTP
└── SECURITY.md
```

Sin dependencias ni paso de build: es HTML y CSS estático.

## Desarrollo local

Sirve la carpeta con cualquier servidor estático (el botón de Google no funciona abriendo el archivo con `file://`):

```bash
npx serve .
# o
python -m http.server 5173
```

## Google Calendar

El botón se configura en `index.html`, dentro del bloque *Google Calendar Appointment Scheduling*:

- `url`: enlace de la página de reservas (Google Calendar → Programación de citas → Compartir).
- `label`: texto del botón.

Si el script de Google no carga (bloqueador de anuncios, red), la página muestra un enlace directo a la misma URL.

El modal de Google trae el iframe con fondo transparente; `css/style.css` le da fondo blanco y un overlay con los colores de la marca. Las reglas usan el selector `iframe[src*="calendar.google.com/calendar/appointments"]` en lugar de las clases internas de Google, que pueden cambiar.

## Deploy

El sitio se publica en **Vercel** desde la rama `main`. Los headers de seguridad (`X-Frame-Options`, `X-Content-Type-Options`, `Referrer-Policy`, `Permissions-Policy`) se definen en `vercel.json`.

## Contribuir

1. Crea una rama desde `main` (`feat/...`, `fix/...`, `chore/...`).
2. Prueba localmente, incluyendo abrir el modal de Google en escritorio y móvil.
3. Abre un Pull Request hacia `main`.

## Licencia

© 2026 GoSoft S.A. de C.V. Todos los derechos reservados.
