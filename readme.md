# CV & Portfolio - Carlos Díaz Girol (DATA)

Portfolio personal y CV online desarrollado con HTML5, CSS3 y JavaScript vanilla (ES6+). Proyecto modular y escalable que combina diseño responsive con funcionalidades dinámicas.

## Descripción del Proyecto

Sitio web profesional que incluye:
- **Página principal** con presentación profesional y proyectos destacados
- **Página de contacto** con formulario funcional
- **Cheatsheets** de HTML con navegación sticky
- **Recursos** organizados por categorías con sistema de tabs
- **Modo oscuro** persistente con localStorage
- **Diseño responsive** adaptable a diferentes dispositivos

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Semántica, accesibilidad y buenas prácticas
- **CSS3**: Custom properties, Flexbox, animaciones y transiciones
- **JavaScript ES6+**: Módulos, template strings, desestructuración
- **FormSubmit**: Servicio de envío de emails sin backend
- **Cloudinary**: CDN para imágenes optimizadas

## 📁 Estructura del Proyecto

```
CVData/
├── index.html              # Página principal
├── contacto.html           # Formulario de contacto
├── recursos.html           # Recursos organizados por tabs
├── cheatsheet-html.html    # Cheatsheet con sticky header
├── css/
│   ├── reset.css           # CSS reset moderno
│   └── styles.css          # Estilos principales con variables CSS
├── js/
│   ├── main.js             # Entry point de la aplicación
│   ├── data/
│   │   └── resources.js    # Datos de recursos
│   ├── templates/
│   │   └── template.js     # Header y footer compartidos
│   └── utils/
│       ├── darkMode.js     # Sistema de modo oscuro
│       ├── menu.js         # Menú hamburguesa responsive
│       ├── skillsList.js   # Generador de skills
│       ├── cheatsheetsList.js
│       └── resourcesGenerator.js.js  # Sistema de tabs
└── readme.md
```

## Características Implementadas

### Sistema de Diseño
- **Variables CSS** para colores y tipografía consistentes
- **Paleta de colores** organizada semánticamente (primary, secondary, accent, highlight, warning)
- **Fuente Google Fonts**: Lato (300, 400, 700)
- **Transiciones suaves** en interacciones (0.3s - 0.5s)

### Modo Oscuro
- Toggle entre modo claro y oscuro
- Persistencia con **localStorage**
- Cambio de icono (☀️ / 🌙)
- Sin flash inicial al cargar
- Transiciones suaves entre temas

### 📱 Responsive Design
- **Mobile-first approach**
- Menú hamburguesa en pantallas pequeñas
- Breakpoints: 650px, 768px
- `scroll-padding-top` para header fijo

### Navegación
- Header y footer compartidos mediante templates
- Rutas relativas compatibles con GitHub Pages
- Navegación sticky en cheatsheets
- Enlaces activos marcados visualmente

### 📋 Sistema de Tabs (Recursos)
- Tabs dinámicas generadas desde datos
- Animación fade-in al cambiar de tab
- Cards clickables completas
- Layout flex con wrap responsive
- Hover effects con elevación

### 📧 Formulario de Contacto
- Integración con **FormSubmit**
- Validación HTML5
- Campos: nombre, email, asunto, mensaje
- Protección anti-spam (honeypot)
- Estilos consistentes con focus states

### Sticky Elements
- Header fijo con `position: fixed`
- Navegación de cheatsheet con `position: sticky`
- Z-index organizado para capas correctas

## Funcionalidades JavaScript

### Modularización
- **ES6 Modules** para organización del código
- Imports/exports para reutilización
- Separación de lógica por responsabilidades

### Generación Dinámica
- **Template strings** para HTML dinámico
- Generación de tabs desde array de datos
- Event listeners dinámicos con delegación

### Gestión de Estado
- **localStorage** para persistencia del tema
- Toggle de clases con `classList.toggle()`
- Estado reactivo en tabs y menú

### Optimizaciones
- Eventos delegados para mejor performance
- Lazy initialization de componentes
- Verificación de existencia de elementos (`&&` operator)

## Características CSS Destacadas

### Variables Personalizadas
```css
--primary: #785082    /* Púrpura */
--secondary: #6990aa  /* Azul grisáceo */
--accent: #8fd1fc     /* Azul claro */
--highlight: #ffda73  /* Amarillo */
--warning: #ff99a7    /* Rosa */
```

### Animaciones
- **fadeIn** para tabs
- **translateY** en hover de cards
- **Transiciones** en colores y transformaciones

### Flexbox
- Layout principal: `flex-direction: column`
- Tabs: `flex-wrap` para responsive
- Cards: `flex: 1 1 300px` para distribución

## Buenas Prácticas Aplicadas

### HTML
- Semántica correcta (`header`, `main`, `section`, `article`, `nav`)
- Atributos `aria-*` para accesibilidad
- Meta tags completos (viewport, charset, description)
- Favicon configurado

### CSS
- **Reset CSS** moderno
- Mobile-first responsive
- BEM-like naming en algunas clases
- Variables para mantenibilidad
- Transiciones smooth

### JavaScript
- ES6+ features (arrow functions, template literals, destructuring)
- Módulos para separación de concerns
- Event delegation
- Código DRY (Don't Repeat Yourself)

## 🔮 Mejoras Futuras Posibles

- [ ] Sistema de routing SPA
- [ ] Lazy loading de imágenes
- [ ] Service Worker para PWA
- [ ] Tests unitarios
- [ ] CI/CD con GitHub Actions
- [ ] Internacionalización (i18n)
- [ ] Modo automático (preferencia del sistema)

## Deployment

Preparado para **GitHub Pages**:
- Rutas relativas configuradas
- Assets en CDN (Cloudinary)
- Sin dependencias de build

##  Autor

**Carlos Díaz Girol (DATA)**  
Fullstack Developer & Tech Educator

- LinkedIn: [carlosdiazgirol](https://www.linkedin.com/in/carlosdiazgirol/)
- GitHub: [CarlosDiazGirol](https://github.com/CarlosDiazGirol)

---
