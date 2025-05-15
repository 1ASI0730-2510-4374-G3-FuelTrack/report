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

<h2>5.2. Landing Page, Services & Applications Implementation</h2>

<h3>5.2.1. Sprint 1</h3>

<h4>5.2.1.1. Sprint Planning 1</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <tr><th><strong>Sprint #</strong></th><td>Sprint 1</td></tr>
  <tr><th><strong>Resumen del Sprint Planning</strong></th><td></td></tr>
  <tr><th><strong>Fecha</strong></th><td>2025-04-26</td></tr>
  <tr><th><strong>Hora</strong></th><td>6:00 PM</td></tr>
  <tr><th><strong>Ubicación</strong></th><td>Google Meet</td></tr>
  <tr><th><strong>Preparado por</strong></th><td>Manuel Angel Sanchez Arenas</td></tr>
  <tr><th><strong>Asistentes a la reunión de planificación</strong></th>
    <td>
      Bryan Ronald Espejo Gamarra,<br>
      Manuel Angel Sanchez Arenas,<br>
      Juan Diego Javier Mondoñedo Rodriguez,<br>
      Diego Vicente Seminario Castillo
    </td>
  </tr>
  <tr><th><strong>Resumen del Sprint 0 (Revisión)</strong></th><td>No hubo Sprint 0 previo.</td></tr>
  <tr><th><strong>Resumen del Sprint 0 (Retrospectiva)</strong></th><td>No hubo Sprint 0 previo.</td></tr>
</table>

<hr>

<h4>Objetivo del Sprint y User Stories</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <tr>
    <th><strong>Ítem</strong></th>
    <th><strong>Descripción</strong></th>
  </tr>
  <tr>
    <td><strong>Objetivo del Sprint 1</strong></td>
    <td>
      Nuestro enfoque está en implementar la versión inicial de la Landing Page de FuelTrack.<br>
      Creemos que entrega una primera aproximación completa de la plataforma a los clientes.<br>
      Esto se confirmará cuando la Landing Page esté desplegada en vivo en GitHub Pages y accesible desde cualquier dispositivo.
    </td>
  </tr>
  <tr>
    <td><strong>Velocidad del Sprint 1</strong></td>
    <td>16 Story Points</td>
  </tr>
  <tr>
    <td><strong>Suma de Story Points</strong></td>
    <td>16</td>
  </tr>
</table>

---

<h4>5.2.1.2. Líderes y Colaboradores por Áreas</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Miembro del equipo (Apellido, Nombre)</th>
      <th>Usuario de GitHub</th>
      <th>Landing Page (L/C)</th>
      <th>Login y Autenticación (L/C)</th>
      <th>Documentación (L/C)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Espejo Gamarra, Bryan Ronald</td>
      <td>SaeBryxn</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Sanchez Arenas, Manuel Angel</td>
      <td>manuels7a</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Mondoñedo Rodriguez, Juan Diego Javier</td>
      <td>Jmondonedor</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Seminario Castillo, Diego Vicente</td>
      <td>DiegoSeminario</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Navarro Correa, César Augusto</td>
      <td>csr555-ui</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
  </tbody>
</table>


### 5.2.1.3. Sprint Backlog 1
**Sprint Objective:**
Implementar funcionalidades básicas para el registro, gestión de pedidos y autenticación de usuarios en FuelTrack.


<h4>Tabla de Sprint Backlog</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Historia de Usuario</th>
      <th>Elemento de trabajo / Tarea</th>
      <th>Descripción</th>
      <th>Estimación (Horas)</th>
      <th>Asignado a</th>
      <th>Estado</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US13</td>
      <td>Implementar visualización del Landing Page</td>
      <td>Mostrar una landing page informativa para que los interesados conozcan la plataforma antes de registrarse.</td>
      <td>5</td>
      <td>Bryan Ronald Espejo Gamarra</td>
      <td>Finalizado</td>
    </tr>
    <tr>
      <td>EP04</td>
      <td>Landing Page informativa y funcional</td>
      <td>Landing page con secciones informativas, beneficios, segmentos y botones que dirigen a login o registro.</td>
      <td>6</td>
      <td>Manuel Angel Sanchez Arenas</td>
      <td>Finalizado</td>
    </tr>
  </tbody>
</table>


<h4>5.2.1.4. Development Evidence for Sprint Review</h4>

<p><strong>Resumen:</strong><br>
Durante este Sprint, el equipo implementó y desplegó con éxito la versión inicial de la Landing Page de FuelTrack. Los commits relacionados con estos avances se detallan a continuación.
</p>

<h4>5.2.1.5. Tabla de Commits</h4>

<p><strong>Resumen:</strong> Esta tabla lista los commits realizados durante los primeros sprints de desarrollo, incluyendo el trabajo en la Landing Page, documentación y configuración del proyecto.</p>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Repositorio</th>
      <th>Rama</th>
      <th>ID de Commit</th>
      <th>Mensaje de Commit</th>
      <th>Descripción del Commit</th>
      <th>Fecha de Commit</th>
    </tr>
  </thead>
<tbody>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>main</td><td>4024b94</td><td>Initial commit</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>develop</td><td>4024b94</td><td>Initial commit</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>4024b94</td><td>Initial commit</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>4024b94</td><td>docs: add initial version of chapter1.md</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>521cd4f</td><td>docs: add initial version of chapter1.md</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>develop</td><td>e1767e7</td><td>Merge pull request #1 from feature/chapter1-introduction</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>develop</td><td>15dd9e2</td><td>Merge pull request #2 from feature/chapter1-introduction</td><td>-</td><td>09/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>c96c7bf</td><td>docs: update introduction with project description and team member profiles</td><td>-</td><td>10/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>1edda67</td><td>feat(assets): add company logo to the report</td><td>-</td><td>10/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>f3d3494</td><td>Update chapter1.md</td><td>Added Lean UX Problem Statement</td><td>12/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>565cf3e</td><td>Update chapter1.md</td><td>Added Lean UX Assumptions</td><td>12/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>6782a2d</td><td>Update chapter1.md</td><td>Added Lean UX Hypothesis statements</td><td>12/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>b2b4e93</td><td>Update chapter1.md</td><td>Added Lean UX Hypothesis statements</td><td>13/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>b64269b</td><td>chapter1 - profile and personal data</td><td>-</td><td>13/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>6aaeb8d</td><td>update - added chapter 2 (competitors/competitive analysis/strategies and tactics against competitors/interview design)</td><td>-</td><td>13/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter1-introduction</td><td>5850634</td><td>docs: refine Lean UX Process with clearer structure and aligned template</td><td>-</td><td>15/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter2-Requirements-Elicitation-&-Analysis</td><td>38aee6c</td><td>3.1 To-Be Scenario</td><td>Added To-Be Scenario</td><td>18/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter2-Requirements-Elicitation-&-Analysis</td><td>1e1693f</td><td>3.2 User stories</td><td>Added section 3.2, with 3 Epics and 12 User Stories.</td><td>18/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter3-Requirements-Specifications</td><td>b2fcfde</td><td>docs: Add Impact Map image</td><td>-</td><td>20/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter3-Requirements-Specifications</td><td>32e7c56</td><td>docs: Update chapter3 Add Impact Map/Product Backlog.md</td><td>-</td><td>20/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter3-Requirements-Specifications</td><td>75af16d</td><td>add: interviews</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>146b38c</td><td>docs: Create chapter4.md</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>ac37eb8</td><td>docs: Create chapter5.md</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>6cc5367</td><td>docs: created asset directory and added database.erd</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>b8859e6</td><td>docs: add Style Guidelines for landing page and branding</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>3e1fe98</td><td>docs: add Information Architecture and navigation systems</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>4bd79dd</td><td>docs: add initial structure for Landing Page UI Design</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>a15affe</td><td>docs: add initial structure for Web Applications UX/UI Design</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>c2c2a26</td><td>docs: add initial structure for Web Applications Prototyping</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>89a0dcb</td><td>docs: add Domain-Driven Software Architecture and C4 diagrams</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>145e64b</td><td>docs: add structure for Software Object-Oriented Design</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>09d785c</td><td>docs: add Database Design and relational diagram</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter4-Product-design</td><td>dd94d03</td><td>docs: added section 4.2.2</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>c2169d0</td><td>feat(docs): add full Chapter 5 structure (Software Configuration Management and Implementation)</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>153ae34</td><td>feat(docs): add Sprint Backlog 1 with assigned tasks</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>a1532b8</td><td>feat(docs): update software configuration and development environment description</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>1d5d90c</td><td>feat(docs): add Execution Evidence with Landing Page screenshots</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>0c8998d</td><td>feat(docs): add Sprint Planning 1 and Aspect Leaders table</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>693b39e</td><td>fix(docs): complete Aspect Leaders and Collaborators table with GitHub usernames</td><td>-</td><td>26/04/2025</td></tr>
  <tr><td>1ASI0730-2510-4374-G3-FuelTrack</td><td>feature/chapter5-Product-Implementation-&-Deployment</td><td>a523d83</td><td>fix(docs): minor corrections and cleanup</td><td>-</td><td>26/04/2025</td></tr>
</tbody>

</table>

---

<h3>5.2.1.5. Execution Evidence for Sprint Review</h3>

<p><strong>Resumen:</strong><br>
Las principales secciones de la Landing Page de FuelTrack fueron desarrolladas y desplegadas exitosamente. A continuación se presentan capturas de pantalla de las secciones implementadas.</p>

<h5>Evidencia de Capturas:</h5>
<ul>
  <li><strong>Hero Section</strong><br><img src="./img/HeroSection.png" alt="Hero Section"></li>
  <li><strong>Features Section 1</strong><br><img src="./img/FeaturesSection1.png" alt="Features Section 1"></li>
  <li><strong>Features Section 2</strong><br><img src="./img/FeaturesSection2.png" alt="Features Section 2"></li>
  <li><strong>Welcome Section</strong><br><img src="./img/WelcomeSection.png" alt="Welcome Section"></li>
  <li><strong>Pricing Section</strong><br><img src="./img/PricingSection.png" alt="Pricing Section"></li>
  <li><strong>Testimonial Section</strong><br><img src="./img/TestimonioSection.png" alt="Testimonial Section"></li>
  <li><strong>Contact Section</strong><br><img src="./img/ContactSection.png" alt="Contact Section"></li>
</ul>

<p><strong>Enlace a Demo en Vivo:</strong><br>
<a href="https://1asi0730-2510-4374-g3-fueltrack.github.io/Landing-page/" target="_blank">FuelTrack Landing Page</a></p>

<hr>

<h4>5.2.1.6. Services Documentation Evidence for Sprint Review</h4>

<!-- Puedes agregar contenido adicional aquí -->

<hr>

<h3>5.2.1.7. Software Deployment Evidence for Sprint Review</h3>

<p><strong>Resumen:</strong><br>
El despliegue inicial de la Landing Page de FuelTrack fue realizado exitosamente utilizando GitHub Pages.</p>

<h5>Detalles del Despliegue:</h5>
<ul>
  <li><strong>URL de la Landing Page:</strong> <a href="https://1asi0730-2510-4374-g3-fueltrack.github.io/Landing-page/" target="_blank">https://1asi0730-2510-4374-g3-fueltrack.github.io/Landing-page/</a></li>
  <li><strong>Repositorio:</strong> <a href="https://github.com/1ASI0730-2510-4374-G3-FuelTrack/Landing-page" target="_blank">https://github.com/1ASI0730-2510-4374-G3-FuelTrack/Landing-page</a></li>
</ul>

<h5>Actividades de Despliegue:</h5>
<ul>
  <li>Configuración del repositorio con GitHub Pages.</li>
  <li>Construcción y despliegue del sitio estático generado con Vite (Vue 3) a la rama <code>gh-pages</code>.</li>
</ul>

<hr>

<h3>5.2.1.8. Team Collaboration Insights during Sprint</h3>

<p><strong>Resumen:</strong><br>
El equipo colaboró mediante GitHub y WhatsApp durante el Sprint. Las actividades principales se centraron en el desarrollo y despliegue de la Landing Page.</p>

<h5>Evidencia de Colaboración:</h5>
<ul>
  <li>Captura de pantalla de commits en GitHub mostrando contribuciones del equipo.</li>
  <li>Conversaciones de WhatsApp sobre coordinación de secciones y ajustes de diseño.</li>
</ul>

<h5>Principales Herramientas de Comunicación:</h5>
<ul>
  <li>GitHub (control de versiones y manejo de issues)</li>
  <li>WhatsApp (comunicación diaria y aclaraciones rápidas)</li>
  <li>Google Meet (reuniones de planificación de sprint)</li>
</ul>


<h3>5.2.2 Sprint 2</h3>

<h4>5.2.2.1. Sprint Planning 2</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <tr><th><strong>Sprint #</strong></th><td>Sprint 2</td></tr>
  <tr><th><strong>Resumen del Sprint Planning</strong></th><td>---</td></tr>
  <tr><th><strong>Fecha</strong></th><td>2025-05-09</td></tr>
  <tr><th><strong>Hora</strong></th><td>11:00 PM</td></tr>
  <tr><th><strong>Ubicación</strong></th><td>Google Meet</td></tr>
  <tr><th><strong>Preparado por</strong></th><td>Manuel Angel Sanchez Arenas</td></tr>
  <tr><th><strong>Asistentes a la reunión de planificación</strong></th>
    <td>
      Bryan Ronald Espejo Gamarra,<br>
      Manuel Angel Sanchez Arenas,<br>
      Juan Diego Javier Mondoñedo Rodríguez,<br>
      Diego Vicente Seminario Castillo<br>
	Cesar Augusto Navarro Correa
    </td>
  </tr>
  <tr><th><strong>Resumen del Sprint 1 (Revisión)</strong></th><td>Creación de un nuevo repositorio para el Landing Page y asignación de tareas para implementar sus funciones para la interacción del usuarios</td></tr>
  <tr><th><strong>Resumen del Sprint 1 (Retrospectiva)</strong></th><td>Realización de la primera versión del Landing Page y el registro de usuario del proveedor y solicitante.</td></tr>
</table>

<hr>

<h4>Objetivo del Sprint y User Stories</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <tr>
    <th><strong>Ítem</strong></th>
    <th><strong>Descripción</strong></th>
  </tr>
  <tr>
    <td><strong>Objetivo del Sprint 2</strong></td>
    <td>
      Nuestro enfoque está en implementar la versión inicial del Frontend de la pagina web de FuelTrack.<br>
      Creemos que esto será un aproximado de como los usuarios van a interactuar y a utilizar la plataforma.<br>
      Esto se confirmará cuando la pagina web esté desplegada en vivo en GitHub Pages y accesible desde cualquier dispositivo.
    </td>
  </tr>
  <tr>
    <td><strong>Velocidad del Sprint 2</strong></td>
    <td> 46 Story Points</td>
  </tr>
  <tr>
    <td><strong>Suma de Story Points</strong></td>
    <td>46</td>
  </tr>
</table>

---

<h4>5.2.2.2. Líderes y Colaboradores por Áreas</h4>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Miembro del equipo (Apellido, Nombre)</th>
      <th>Usuario de GitHub</th>
      <th>Landing Page (L/C)</th>
      <th>Login y Autenticación (L/C)</th>
      <th>Documentación (L/C)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Espejo Gamarra, Bryan Ronald</td>
      <td>SaeBryxn</td>
      <td>L</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Sanchez Arenas, Manuel Angel</td>
      <td>manuels7a</td>
      <td>C</td>
      <td>L</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Mondoñedo Rodriguez, Juan Diego Javier</td>
      <td>Jmondonedor</td>
      <td>C</td>
      <td>C</td>
      <td>L</td>
    </tr>
    <tr>
      <td>Seminario Castillo, Diego Vicente</td>
      <td>DiegoSeminario</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
    <tr>
      <td>Navarro Correa, César Augusto</td>
      <td>csr555-ui</td>
      <td>C</td>
      <td>C</td>
      <td>C</td>
    </tr>
  </tbody>
</table>


### 5.2.2.3. Sprint Backlog 2
**Sprint Objective:**
Implementar funcionalidades básicas para el registro, gestión de pedidos y autenticación de usuarios en FuelTrack.


<h4>Tabla de Sprint Backlog</h4>

<h4>5.2.1.4. Development Evidence for Sprint Review</h4>

<p><strong>Resumen:</strong><br>

</p>

<h4>5.2.1.5. Tabla de Commits</h4>


---

<h3>5.2.1.5. Execution Evidence for Sprint Review</h3>

<p><strong>Resumen:</strong><br>

<h5>Evidencia de Capturas:</h5>

<h4>5.2.2.6. Services Documentation Evidence for Sprint Review</h4>

<hr>

<h3>5.2.2.7. Software Deployment Evidence for Sprint Review</h3>


<h3>5.2.1.8. Team Collaboration Insights during Sprint</h3>

