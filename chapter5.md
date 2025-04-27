# 5.1. Software Configuration Management

## 5.1.1. Software Development Environment Configuration

**Project Management:**
- **WhatsApp**: Aplicación de mensajería instantánea propiedad de Meta, utilizada para coordinar tareas del equipo y facilitar el intercambio de ideas y apoyo continuo durante el desarrollo del proyecto.
- **Google Meet**: Herramienta de videoconferencias de Google, usada para mantener reuniones virtuales, planificación de tareas y comunicación directa.
- **Google Drive**: Servicio de almacenamiento en la nube para compartir archivos relevantes y documentación del proyecto entre los miembros del equipo.

**Requirements Management:**
- **UXPressia**: Utilizada para la creación de User Personas, User Journey Maps e Impact Maps, mejorando la comprensión de las necesidades del usuario.
- **Zoom**: Empleada para la realización de entrevistas de necesidad y validación de usuarios potenciales.

**Product UX/UI Design:**
- **Figma**: Plataforma colaborativa para el diseño de wireframes, wireflows, mockups y prototipos interactivos.

**Software Development:**
- **Vertabelo**: Herramienta para el diseño del modelo de base de datos, asegurando una estructura visual clara de entidades y relaciones.
- **Google Chrome**: Navegador utilizado para realizar pruebas de compatibilidad y funcionalidad de la Landing Page y Web Application.
- **Visual Studio Code**: Editor de código para programar en JavaScript, Vue.js, y gestionar el control de versiones mediante GitHub.

**Software Documentation:**
- **Google Docs**: Documentos colaborativos para registrar decisiones, avances y acuerdos del proyecto.
- **Structurizr**: Herramienta para diseñar diagramas C4, representando arquitecturas de software a distintos niveles de abstracción.

## 5.1.2. Source Code Management

El proyecto utiliza GitHub como repositorio para administrar y estructurar los avances. Implementamos el flujo de trabajo **Gitflow**, siguiendo la metodología propuesta por Vincent Driessen, para mantener versiones estables y trabajo colaborativo ordenado.

**Main branch:** Rama principal donde se almacena el código de producción estable.

**Develop branch:** Rama de integración donde se fusionan las nuevas funcionalidades desarrolladas.

**Feature branches:** Ramas creadas a partir de `develop` para desarrollar funcionalidades específicas. Cada feature se trabaja de forma aislada para evitar conflictos.

**Conventional Commits:** Estándar aplicado en los mensajes de commit para mantener un historial de cambios claro, comprensible y trazable, mejorando además la automatización de flujos de despliegue.

## 5.1.3. Source Code Style Guide & Conventions

Nuestro equipo adoptó las siguientes convenciones de estilo para los lenguajes utilizados, buscando mantener la consistencia, la legibilidad y la facilidad de mantenimiento del código.

**HTML:**
- Elementos y atributos en minúsculas.
- Cierre explícito de todas las etiquetas.
- Inclusión de atributos requeridos como `alt` en imágenes y `id`, `name` en formularios.
- Código estructurado para mejorar la legibilidad.

**CSS:**
- Uso de nombres de clases en kebab-case.
- Espaciado consistente y cierre obligatorio de declaraciones con punto y coma.
- Organización modular de reglas CSS.

**JavaScript / Vue.js:**
- Declaración de variables con `const` y `let`.
- Componentes Vue nombrados usando PascalCase (`OrderForm.vue`).
- Estructura de componentes siguiendo el orden `template`, `script`, `style`.
- Código y comentarios en inglés.
- Uso de programación funcional, separación de responsabilidades, y aplicación de mejores prácticas recomendadas por la [Vue 3 Style Guide](https://vuejs.org/style-guide/).

## 5.1.4. Software Deployment Configuration

**Entorno de Desarrollo:**

Tecnologías utilizadas:
- HTML5
- CSS3
- JavaScript
- Vue 3 (con Vite como empaquetador y servidor de desarrollo)

Gestor de paquetes:
- **npm** para Vue 3 (administración de dependencias y scripts de build).

**Estrategia de Deployment:**
- **GitHub Pages** para desplegar la versión estática del Landing Page.
- **Azure App Services** para desplegar los servicios backend (API RESTful).

**Flujo Gitflow aplicado:**
- `main`: Rama principal de producción.
- `develop`: Rama de integración principal.
- `feature/*`: Desarrollo de nuevas funcionalidades sobre `develop`.
- Pull Requests realizados desde `feature/*` hacia `develop`, y de `develop` hacia `main` al completar un ciclo.

# 5.2. Landing Page, Services & Applications Implementation

## 5.2.1. Sprint 1

### 5.2.1.1. Sprint Planning 1

| **Sprint #** | Sprint 1 |
|:-------------|:---------|
| **Sprint Planning Background** | |
| **Date** | 2025-04-26 |
| **Time** | 6:00 PM |
| **Location** | Google Meet |
| **Prepared By** | Manuel Angel Sanchez Arenas |
| **Attendees (to planning meeting)** | Bryan Ronald Espejo Gamarra, Manuel Angel Sanchez Arenas, Juan Diego Javier Mondoñedo Rodriguez, Diego Vicente Seminario Castillo |
| **Sprint 0 Review Summary** | No hubo Sprint 0 previo. |
| **Sprint 0 Retrospective Summary** | No hubo Sprint 0 previo. |

---

**Sprint Goal & User Stories**

| Item | Description |
|:-----|:------------|
| **Sprint 1 Goal** | Our focus is on implementing the FuelTrack Landing Page initial version.<br>We believe it delivers a complete first approach of the platform to customers.<br>This will be confirmed when the Landing Page is deployed live on GitHub Pages and accessible from any device. |
| **Sprint 1 Velocity** | 16 Story Points |
| **Sum of Story Points** | 16 |

---

### 5.2.1.2. Aspect Leaders and Collaborators

| Team Member (Last Name, First Name) | GitHub Username | Landing Page (L/C) | Login & Authentication (L/C) | Documentation (L/C) |
|:------------------------------------|:----------------|:-------------------|:-----------------------------|:--------------------|
| Sanchez Arenas, Manuel Angel | (coloca tu username) | L | C | C |
| Espejo Gamarra, Bryan Ronald | (coloca tu username) | C | L | C |
| Mondoñedo Rodriguez, Juan Diego Javier | (coloca tu username) | C | C | L |
| Seminario Castillo, Diego Vicente | (coloca tu username) | C | C | C |

---
### 5.2.1.3. Sprint Backlog 1
**Sprint Objective:**
Implementar funcionalidades básicas para el registro, gestión de pedidos y autenticación de usuarios en FuelTrack.


**Sprint Backlog Table:**

| User Story | Work-Item / Task | Description | Estimation (Hours) | Assigned To | Status |
|:----------|:-----------------|:------------|:-------------------|:------------|:-------|
| US01 | Implement Create New Order Page | Crear la interfaz de formulario para registrar nuevos pedidos de combustible | 6 | Bryan Ronald Espejo Gamarra | In-Process |
| US02 | Develop Order History Page | Crear pantalla donde se pueda consultar historial de pedidos con filtros | 5 | Manuel Angel Sanchez Arenas | In-Process |
| US03 | Add Edit Order Functionality | Permitir edición/cancelación de pedidos antes de ser confirmados | 5 | Juan Diego Javier Mondoñedo Rodriguez | In-Process |
| US04 | Create Order Confirmation Panel (Provider) | Vista donde proveedores confirmen o rechacen pedidos recibidos | 4 | Diego Vicente Seminario Castillo | In-Process |
| US05 | Enable Order Status Update | Permitir actualizar el estado de pedidos en panel del proveedor | 4 | Bryan Ronald Espejo Gamarra | In-Process |
| US06 | Configure Client Notifications | Implementar envío de notificaciones al cliente en cambios de pedidos | 3 | Manuel Angel Sanchez Arenas | In-Process |
| US08 | Implement Login Page | Construir vista de inicio de sesión para usuarios | 4 | Juan Diego Javier Mondoñedo Rodriguez | In-Process |
| US09 | Develop User Registration Page | Implementar registro de cuenta (cliente o proveedor) con validaciones | 5 | Diego Vicente Seminario Castillo | In-Process |
| US10 | Add Password Recovery Functionality | Crear flujo de recuperación de contraseña vía correo electrónico | 3 | Bryan Ronald Espejo Gamarra | In-Process |
| US11 | Apply Role-Based Access Control | Asegurar restricciones de acceso según el rol de usuario | 3 | Manuel Angel Sanchez Arenas | In-Process |
| US12 | Setup MFA Authentication for Orders | Añadir autenticación de segundo factor en el envío de pedidos | 6 | Juan Diego Javier Mondoñedo Rodriguez | In-Process |

### 5.2.1.4. Development Evidence for Sprint Review

**Summary:**
During this Sprint, the team successfully implemented and deployed the initial version of the FuelTrack Landing Page. The commits related to these advancements are listed below.

**Commits Table:**

| Repository | Branch | Commit ID | Commit Message | Commit Message Body | Committed on (Date) |
|:-----------|:-------|:-----------|:---------------|:--------------------|:--------------------|
| SaeBryxn/LandigPageFuelTrack | main | a6919063b377e88e43fa04460407149b66800b6e | add: initial up landing page | Initial deployment of the Landing Page including basic sections (hero, features, contact). | 26/04/2025 |


*(You should replace commit ID and date with your real commit info from GitHub.)*

---

### 5.2.1.5. Execution Evidence for Sprint Review

**Summary:**
The main features of the FuelTrack Landing Page were developed and deployed successfully. Below are screenshots of the implemented sections.

**Screenshots Evidence:**

- **Hero Section**  
  ![Hero Section](./img/HeroSection.png)

- **Features Section 1**  
  ![Features Section 1](./img/FeaturesSection1.png)

- **Features Section 2**  
  ![Features Section 2](./img/FeaturesSection2.png)

- **Welcome Section**  
  ![Welcome Section](./img/WelcomeSection.png)

- **Pricing Section**  
  ![Pricing Section](./img/PricingSection.png)

- **Testimonial Section**  
  ![Testimonial Section](./img/TestimonioSection.png)

- **Contact Section**  
  ![Contact Section](./img/ContactSection.png)

**Live Demo Link:**
- [FuelTrack Landing Page](https://saebryxn.github.io/LandigPageFuelTrack/)

---

### 5.2.1.6. Services Documentation Evidence for Sprint Review

*(Not applicable yet: No backend services developed in this Sprint.)*

---

### 5.2.1.7. Software Deployment Evidence for Sprint Review

**Summary:**
The initial deployment of the FuelTrack Landing Page was completed using GitHub Pages.

**Deployment Details:**
- **Landing Page URL:** [https://saebryxn.github.io/LandigPageFuelTrack/](https://saebryxn.github.io/LandigPageFuelTrack/)
- **Repository URL:** [https://github.com/SaeBryxn/LandigPageFuelTrack](https://github.com/SaeBryxn/LandigPageFuelTrack)

**Deployment Activities:**
- Configured GitHub repository with GitHub Pages hosting.
- Built and pushed static site generated with Vite (Vue 3) to `gh-pages`.

---

### 5.2.1.8. Team Collaboration Insights during Sprint

**Summary:**
The team collaborated via GitHub and WhatsApp during this Sprint. The main activities focused on the development and deployment of the Landing Page.

**Collaboration Evidence:**
- Screenshot of GitHub commits showing contribution by team members.
- WhatsApp conversations coordinating Landing Page sections and design adjustments.

**Main Communication Tools:**
- GitHub (code versioning and issues)
- WhatsApp (daily communication and quick clarifications)
- Google Meet (sprint planning meetings)

---
