# GoSoft Calendar - Landing Page de Citas

Una landing page moderna y profesional para el sistema de programación de citas de GoSoft Solutions, integrada con Google Calendar.

## Características

- 🎯 **Landing Page Informativa**: Diseño limpio y profesional enfocado en la programación de citas
- 📅 **Integración Google Calendar**: Botón de programación directa con Google Calendar
- 📱 **Diseño Responsive**: Optimizado para dispositivos móviles y desktop
- ⚡ **Carga Rápida**: HTML, CSS y JavaScript vanilla para máximo rendimiento
- 🎨 **Diseño Moderno**: Interfaz atractiva con colores corporativos

## Estructura del Proyecto

```
gosoft-calendar/
├── index.html              # Página principal
├── css/
│   └── style.css           # Estilos principales
├── .github/
│   └── copilot-instructions.md
└── README.md               # Este archivo
```

## Instalación y Uso

1. **Clonar o descargar el proyecto**
   ```bash
   git clone <repository-url>
   cd gosoft-calendar
   ```

2. **Abrir la landing page**
   - Abrir `index.html` en cualquier navegador web moderno
   - O usar Live Server en VS Code para desarrollo

3. **Personalización**
   - Modificar colores en `css/style.css`
   - Actualizar información de contacto en `index.html`
   - Reemplazar URL de Google Calendar con la tuya propia

## Configuración de Google Calendar

El proyecto incluye la integración con Google Calendar usando el script oficial. Para usar tu propio calendario:

1. Ve a Google Calendar
2. Crea un enlace de programación de citas
3. Reemplaza la URL en el script del archivo `index.html`:

```javascript
url: 'TU_URL_DE_GOOGLE_CALENDAR_AQUÍ',
```

## Personalización

### Colores
Los colores principales se pueden modificar en `css/style.css`:
- Azul principal: `#039BE5`
- Azul secundario: `#0277BD`

### Contenido
- **Título**: Modificar en la etiqueta `<h1>` del header
- **Descripción**: Actualizar en la sección hero
- **Beneficios**: Editar las tarjetas en la sección info
- **Contacto**: Actualizar información en la sección contact-info

## Tecnologías Utilizadas

- **HTML5**: Estructura semántica
- **CSS3**: Estilos modernos con Flexbox y Grid
- **JavaScript**: Integración con Google Calendar API
- **Google Calendar Scheduling**: Sistema de citas integrado

## Estructura de Secciones

1. **Header**: Logo y navegación
2. **Hero**: Título principal y botón de cita
3. **Información**: Beneficios de agendar reunión
4. **Contacto**: Información de contacto de la empresa
5. **Footer**: Copyright y información adicional

## Soporte de Navegadores

- Chrome 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## Licencia

© 2026 GoSoft Solutions. Todos los derechos reservados.

## Contacto

Para soporte técnico o consultas:
- **Email**: info@gosoftsolutions.com
- **Teléfono**: +1 (555) 123-4567