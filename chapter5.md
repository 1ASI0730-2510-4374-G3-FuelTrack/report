
# 5.1. Software Configuration Management

## 5.1.1. Software Development Environment Configuration

**Project Management:**
- **Trello**: Gestión de tareas por sprint, asignación de tareas y seguimiento de avance.
- **GitHub**: Plataforma para el control de versiones y gestión de repositorios.
- **Microsoft Teams**: Comunicación continua del equipo para reuniones virtuales y coordinación diaria.

**Requirements Management:**
- **UXPressia**: Elaboración de User Personas, User Journey Maps e Impact Maps.
- **Google Forms**: Recopilación de información para entrevistas de validación y necesidad.

**Product UX/UI Design:**
- **Figma**: Diseño de wireframes, mockups, prototipos interactivos para el Landing Page y Web Application.

**Software Development:**
- **Visual Studio Code**: Editor principal de código para desarrollo en Vue, HTML5, CSS3 y JavaScript.
- **Google Chrome**: Navegador usado para pruebas de visualización y compatibilidad.
- **Postman**: Pruebas de los endpoints del API RESTful.

**Software Documentation:**
- **Structurizr**: Elaboración de diagramas de arquitectura de software (modelo C4).
- **Swagger (OpenAPI)**: Documentación interactiva de los servicios web.
- **Markdown (.md)**: Documentación del proyecto en repositorio GitHub.

## 5.1.2. Source Code Management

**Plataforma:**
- **GitHub** (Organización pública).

**Estrategia de control de versiones:**
- **GitFlow** basado en el modelo de Vincent Driessen:
  - `main`: Rama de producción estable.
  - `develop`: Rama de integración.
  - `feature/*`: Ramas para nuevas funcionalidades.
  - `release/*`: Ramas para preparar versiones de lanzamiento.
  - `hotfix/*`: Ramas para solucionar bugs críticos.

**Normas de commits:**
- **Conventional Commits** (feat, fix, docs, refactor, chore, etc.).

**Versionado:**
- **Semantic Versioning 2.0.0** (ejemplo: v1.2.3).

## 5.1.3. Source Code Style Guide & Conventions

**HTML:**
- Uso de minúsculas para etiquetas y atributos.
- Cierre obligatorio de etiquetas.
- Atributos `alt` en imágenes y `name/id` en formularios.

**CSS:**
- Clases en kebab-case (`.landing-section`).
- Propiedades agrupadas lógicamente.
- Espacios y saltos de línea para mejorar legibilidad.

**JavaScript (Vue.js):**
- Uso de `const` y `let`.
- Componentes pequeños y especializados.
- Código y comentarios en inglés.

**Vue.js:**
- PascalCase para nombres de componentes (`LandingPage.vue`).
- Estructura interna: `template`, `script`, `style` en orden.
- Aplicación de la [Guía de Estilo Oficial de Vue](https://vuejs.org/style-guide/).

## 5.1.4. Software Deployment Configuration

**Entorno de desarrollo:**
- **HTML5, CSS3, JavaScript, Vue 3 (con Vite).**
- **ASP.NET Core (API RESTful).**

**Gestores de paquetes:**
- `npm` para Vue.js.
- `nuget` para ASP.NET Core.

**Plataformas de despliegue:**
- **GitHub Pages** para el Landing Page.
- **Azure App Services** para el API RESTful.

**Flujo de despliegue:**
- Pull Request de `feature/*` hacia `develop`.
- Validación y merge de `develop` hacia `main`.
- Publicación automática mediante GitHub Actions.

# 5.2. Landing Page, Services & Applications Implementation

## 5.2.1. Sprint 1

### 5.2.1.1. Sprint Planning 1

| **Sprint #** | Sprint 1 |
|--------------|----------|
| **Sprint Planning Background** | |
| **Date** | 10/04/2025 |
| **Time** | 11:00 AM |
| **Location** | Microsoft Teams |
| **Prepared By** | Ingrese nombre aquí |
| **Attendees** | Ingrese nombres aquí |
| **Sprint 0 Review Summary** | No hubo sprint previo |
| **Sprint 0 Retrospective Summary** | No hubo sprint previo |
| **Sprint Goal** | Desplegar la primera versión del Landing Page y configurar repositorios |
| **Sprint 1 Velocity** | 16 |
| **Sum of Story Points** | 16 |

---

### 5.2.1.2. Aspect Leaders and Collaborators

| Aspect | Leader | Collaborators |
|--------|--------|---------------|
| Frontend Development (Landing Page) | Ingrese nombre aquí | Todos los miembros |
| UI/UX Design | Ingrese nombre aquí | Todos los miembros |
| Code Repository & Gitflow | Ingrese nombre aquí | Todos los miembros |
| Deployment & Hosting | Ingrese nombre aquí | Todos los miembros |
| Documentation & Markdown | Ingrese nombre aquí | Todos los miembros |


### 5.2.1.3. Sprint Backlog 1

- Creación del repositorio y configuración inicial.
- Diseño de wireframes del Landing Page.
- Desarrollo del Landing Page en Vue 3 + Vite.
- Hosting en GitHub Pages.
- Redacción inicial del informe en Markdown.

### 5.2.1.4 a 5.2.1.8