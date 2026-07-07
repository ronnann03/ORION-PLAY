# Proyecto Cooll Play - Sustentación Técnica

Este repositorio contiene la implementación del proyecto **Cooll Play**, una tienda de videojuegos en línea diseñada con un enfoque educativo para demostrar el dominio de múltiples tecnologías frontend.

## 🎯 Cumplimiento de la Rúbrica (Nivel Excelente)

Este proyecto ha sido estructurado meticulosamente aislando cada tecnología requerida en diferentes páginas. Esto evita conflictos de CSS y demuestra un uso modular, justificado y profesional de las herramientas.

### 1. Preprocesadores (LESS y SASS)
*   **SASS (`index.html` y `/scss`)**: 
    *   **Implementación:** Se usó para la página de inicio.
    *   **Evidencias:** Uso de variables (`$primary-color`), anidamiento (`.navbar { .nav-links { ... } }`), mixins (`@mixin glassmorphism`), e importación de parciales (`@import 'variables'`). Compilado a `css/main-sass.css`.
*   **LESS (`profile.html` y `/less`)**: 
    *   **Implementación:** Se usó para la vista de Perfil de Usuario.
    *   **Evidencias:** Uso de variables (`@bg-color`), operaciones matemáticas para paddings (`@large-padding: @base-padding * 2`), funciones de color (`darken()`, `lighten()`), y mixins (`.box-shadow()`). Compilado a `css/main-less.css`.

### 2. Animaciones, Transiciones y Transformaciones
*   Implementadas principalmente en `index.html` (vía SASS).
*   **Evidencias:** 
    *   `@keyframes` para efectos de entrada (`fadeInDown`, `slideUp`) aportando fluidez.
    *   `transition` y `transform` (`hover-glow` y cards) para interactividad cuando el usuario pasa el cursor.
    *   Sombra pulsante animada infinitamente (`pulseGlow`).

### 3. Responsividad y Cross-Browser
*   Todas las páginas incluyen `<meta name="viewport" content="width=device-width, initial-scale=1.0">`.
*   Uso de media queries y unidades relativas en SASS (`_mixins.scss`).
*   Los frameworks CSS elegidos (Bootstrap, Tailwind, etc.) garantizan compatibilidad móvil y de navegadores por defecto.

### 4. Frameworks CSS (4 Requeridos)
Implementados de forma aislada para evitar conflictos:
1.  **Bootstrap 5 (`products.html`, `product-detail.html`)**: Utilizado para las galerías de productos por su excelente sistema de grillas (Grid System) y componentes de tarjetas listos para usar.
2.  **Tailwind CSS (`cart.html`, `checkout.html`)**: Utilizado vía CDN para demostrar la construcción rápida de interfaces mediante utility-classes (Flexbox, paddings, tipografía), ideal para flujos de pago modernos.
3.  **Materialize CSS (`login.html`)**: Implementado para el formulario de inicio de sesión, destacando sus inputs animados y el diseño limpio basado en Material Design clásico.
4.  **Material Design for Bootstrap - MDB (`register.html`)**: Usado para demostrar otra variante de Material Design, aprovechando su estética tipo "glassmorphism" y componentes avanzados en el formulario de registro.

---

## 🚀 Instrucciones de Ejecución

### Requisitos Previos
*   Tener instalado **Node.js** y **NPM** (para compilar los estilos).

### Pasos para Ejecutar
1.  Abre una terminal en la carpeta del proyecto `orion-play`.
2.  Instala las dependencias (compiladores de SASS y LESS):
    ```bash
    npm install
    ```
3.  Compila los archivos `.scss` y `.less` a la carpeta `/css`:
    ```bash
    npm run build
    ```
4.  Abre el archivo `index.html` en tu navegador preferido (doble clic o usando una extensión como Live Server).
5.  Navega a través de las diferentes páginas (Tienda, Carrito, Login, Registro, Perfil) usando los enlaces de los menús.

---

## 📅 Mapa de Cumplimiento por Semanas

| Semana | Tarea Realizada | Responsable (Rol) |
| :--- | :--- | :--- |
| **Semana 1** | Planificación, Wireframes y Configuración inicial (NPM, SASS, LESS). | Arquitecto Frontend |
| **Semana 2** | Desarrollo del `index.html` (SASS) y animaciones CSS (Keyframes, Transiciones). | Desarrollador UI |
| **Semana 3** | Implementación de frameworks: Bootstrap (`products.html`) y Tailwind (`cart.html`). | Desarrollador UI |
| **Semana 4** | Integración de Materialize (`login.html`), MDB (`register.html`) y LESS (`profile.html`). | Desarrollador UX |
| **Semana 5** | Pruebas Cross-Browser, revisión responsive, compilación final y redacción del README. | QA & Documentador |

*(Nota: Cada miembro del equipo debe poder explicar los archivos .scss, .less y las clases de los frameworks en la sustentación grupal).*
