# Capítulo II: Requirements Elicitation & Analysis 
## 2.1. Competidores.

PetroApp es una plataforma digital que facilita la compra y venta de combustible, principalmente orientada a consumidores finales y estaciones de servicio. Permite ubicar estaciones cercanas, gestionar pagos electrónicos y controlar el consumo desde una app. Esta enfocada principalmente en el uso personal, pero también ofrece soluciones para empresas, con funcionalidades que permiten cierta trazabilidad y control, aunque con menos enfoque en el flujo completo del pedido corporativo.

FuelCloud es una solución tecnológica centrada en el control del despacho de combustible mediante una combinación de hardware y software. Este ofrece monitoreo en tiempo real, control de acceso al combustible, reportes detallados de consumo y ubicación, lo que la hace ideal para empresas con tanques propios. Además, se enfoca más en el control físico del combustible que en la gestión administrativa o logística del pedido entre proveedor y cliente.

Wialon es una plataforma global de gestión de flotas que incluye funcionalidades para el control de combustible, seguimiento de vehículos por GPS, y análisis de consumo. Ofrece herramientas de visualización en tiempo real, alertas automatizadas y reportes avanzados. Si bien no gestiona directamente el flujo de pedidos entre proveedores y solicitantes, es altamente utilizada por empresas distribuidoras y logísticas que transportan combustible, lo que la convierte en un competidor indirecto pero funcionalmente cercano a FuelTrack.

### 2.1.1. Análisis competitivo.
<table border="1">
  <tr>
    <th colspan="6" style="text-align:left">Competitive Analysis Landscape</th>
  </tr>
  <tr>
    <td><strong>¿Por qué llevar a cabo este análisis?</strong></td>
    <td colspan="5">Este análisis se está llevando a cabo porque queremos conocer las ventajas y desventajas de nuestra aplicación frente a la competencia, y cómo nos diferenciamos de ellas.</td>
  </tr>
  <tr>
  <td colspan="2"><strong>(En la cabecera colocar por cada competidor nombre y logo)</strong></td>
  <td><strong>FuelTrack</strong><br><img src="img/logo-fueltrack.jpg" height="120"/></td>
  <td><strong>Zavgar</strong><br><img src="img/logo-zavgar.jpg" height="120"/></td>
  <td><strong>FuelCloud</strong><br><img src="img/logo-fuelcloud.jpg" height="120"/></td>
  <td><strong>Wialon</strong><br><img src="img/logo-wialon.jpg" height="120"/></td>
</tr>

  <tr>
    <th rowspan="3">Perfil</th>
    <td><strong>Visión general</strong></td>
    <td>Plataforma web que digitaliza y estructura el proceso completo de pedido de combustible entre empresas y proveedores.</td>
    <td>SaaS para la gestión de consumo de combustible de flotas, con enfoque en eficiencia, monitoreo y costos.</td>
    <td>Solución con hardware/software para el control físico del despacho de combustible.</td>
    <td>Plataforma de gestión de flotas con control de combustible, GPS y reportes operativos.</td>
  </tr>
  <tr>
    <td><strong>Ventaja competitiva</strong></td>
    <td>Especialización en el flujo completo de pedido, despacho y análisis; integración de pagos y logística; UI intuitiva.</td>
    <td>No requiere hardware; ofrece métricas, control de gastos y reportes sobre consumo.</td>
    <td>Control físico preciso del combustible, monitoreo en tiempo real.</td>
    <td>Seguimiento en tiempo real, visualización de rutas, integración con sensores de combustible.</td>
  </tr>
  <tr>
    <td><strong>¿Qué valor ofrece al cliente?</strong></td>
    <td>Trazabilidad total, eficiencia operativa, reportes de consumo y validación segura de pedidos.</td>
    <td>Optimización de costos y control sobre el uso de combustible en flotas.</td>
    <td>Seguridad y precisión operativa en el control de combustible.</td>
    <td>Trazabilidad de flotas, alertas automáticas, análisis de rutas y consumo de combustible.</td>
  </tr>
  <tr>
    <th rowspan="2">Perfil de Marketing</th>
    <td><strong>Mercado objetivo</strong></td>
    <td>Empresas que solicitan combustible a proveedores.</td>
    <td>Empresas con flotas vehiculares que desean monitorear y reducir el consumo de combustible.</td>
    <td>Empresas con tanques de combustible propios.</td>
    <td>Empresas logísticas, distribuidoras y de transporte de combustible.</td>
  </tr>
  <tr>
    <td><strong>Estrategias de marketing</strong></td>
    <td>Alianzas con proveedores, demostraciones de ahorro, marketing de contenido enfocado en eficiencia.</td>
    <td>Enfoque digital, contenido técnico, integración con proveedores de tarjetas de combustible.</td>
    <td>Ferias industriales, distribuidores, venta consultiva entre empresas.</td>
    <td>Alianzas con distribuidores de GPS, marketing técnico, ferias de transporte.</td>
  </tr>
  <tr>
    <th rowspan="3">Perfil de Producto</th>
    <td><strong>Productos & Servicios</strong></td>
    <td>Plataforma para gestión completa de pedidos, seguimiento, reportes, validación y alertas.</td>
    <td>Plataforma web con módulo de abastecimiento, reportes de consumo, integración GPS y tarjetas.</td>
    <td>Hardware IoT y software para gestión, y control de combustible.</td>
    <td>Plataforma SaaS + app móvil con monitoreo, alertas, mapas y módulos personalizables.</td>
  </tr>
  <tr>
    <td><strong>Precios & Costos</strong></td>
    <td>Modelo SaaS con suscripción escalable según volumen y servicios.</td>
    <td>SaaS con modelos por flota activa o vehículos monitoreados.</td>
    <td>Venta e instalación de hardware + licencias de software.</td>
    <td>Modelo SaaS modular, basado en vehículos activos y funcionalidades activadas.</td>
  </tr>
  <tr>
    <td><strong>Canales de distribución</strong></td>
    <td>Web app responsive, potencial app móvil futura.</td>
    <td>Web app, marketing digital y comunidad de flotas.</td>
    <td>Plataforma web + hardware instalado en sitio.</td>
    <td>Red de partners global, distribuidores locales e integradores de sistemas GPS.</td>
  </tr>
  <tr>
    <th rowspan="4">Análisis SWOT</th>
    <td><strong>Fortalezas</strong></td>
    <td>Enfoque especializado, experiencia de usuario optimizada, integraciones clave, análisis avanzado de consumo.</td>
    <td>Implementación ágil, sin hardware, fácil adopción en empresas medianas.</td>
    <td>Control físico riguroso, solución probada en industrias exigentes.</td>
    <td>Plataforma robusta, cobertura internacional, integración con más de 2,400 dispositivos GPS.</td>
  </tr>
  <tr>
    <td><strong>Debilidades</strong></td>
    <td>Nueva en el mercado, menor reconocimiento de marca, necesita consolidar confianza.</td>
    <td>No gestiona el flujo completo del pedido, enfoque parcial en flotas.</td>
    <td>Alto costo, dependencia de hardware, menor adaptabilidad en mercados emergentes.</td>
    <td>No gestiona pedidos entre proveedor y solicitante, requiere configuración técnica inicial.</td>
  </tr>
  <tr>
    <td><strong>Oportunidades</strong></td>
    <td>Alta informalidad en el sector, digitalización creciente en logística, necesidad de trazabilidad y control.</td>
    <td>Mayor conciencia en eficiencia de flotas y digitalización de costos operativos.</td>
    <td>Nuevos mercados industriales con enfoque en seguridad y control.</td>
    <td>Creciente necesidad de control logístico y monitoreo de distribución en países en desarrollo.</td>
  </tr>
  <tr>
    <td><strong>Amenazas</strong></td>
    <td>Aparición de soluciones similares, resistencia al cambio en empresas tradicionales, competencia ERP.</td>
    <td>SaaS especializados con mayor cobertura funcional (ERP, proveedores, logística).</td>
    <td>SaaS ágiles y sin hardware físico, que ofrecen soluciones más accesibles.</td>
    <td>SaaS más específicos y ligeros, enfocados exclusivamente en la trazabilidad de entregas.</td>
  </tr>
</table>


### 2.1.2. Estrategias y tácticas frente a competidores.

#### a. Diferenciación a través de especialización
Una de las principales estrategias de **FuelTrack** es la **especialización en el flujo completo de pedido de combustible**. A diferencia de soluciones como **Zavgar**, que están orientadas principalmente al control y análisis del consumo de combustible en flotas, nuestra plataforma se enfoca en las **interacciones B2B** entre empresas solicitantes y proveedores. Esto nos permite ofrecer un **control dedicado del pedido**, **gestión de la logística**, y **reportes detallados de consumo y entregas**, lo cual no está presente en la mayoría de las plataformas competidoras.

- **Táctica**: Desarrollar funcionalidades para la **validación automática de pagos**, **gestión de stock en tiempo real** y la **optimización del transporte** logrando la automatización de procesos que solo eran logrados de forma manual. Esto crea una ventaja frente a competidores como **FuelCloud**, que se centran más en el control físico del combustible y menos en la administración a nivel operativo.

#### b. Innovación en la interfaz de usuario y experiencia

El sistema de **FuelTrack** está diseñado para ofrecer una **experiencia de usuario optimizada**, algo que **Wialon**, **FuelCloud** y la propia **OSINERGMIN** no abordan en sus plataformas. Al ser una solución especializada y dirigida a una tarea específica, podemos dedicar más recursos en crear una interfaz intuitiva y procesos bien definidos brindando comodidad y seguridad a nuestros usuarios.

- **Táctica**: Diseñar una **interfaz intuitiva y consistente** que permita a los usuarios acceder a reportes de consumo, validar pedidos y coordinar logística con facilidad. Además, ofrecer **soporte y formación continua** para asegurar que los usuarios aprovechen al máximo todas las funcionalidades del sistema.

#### c. Flexibilidad en precios y modelo SaaS escalable
El modelo de precios de **FuelTrack** ofrece **planes escalables basados en suscripción**, lo que hace que sea más accesible para medianas y grandes empresas. Esto es más competitivo frente a **Wialon**, que puede no ser una opción viable para empresas que solo requieren una solución de pedidos de combustible. También es más asequible que **FuelCloud**, que requiere una inversión considerable en hardware, instalación y mantenimiento.

- **Táctica**: Ofrecer un modelo de suscripción flexible y **precios competitivos**, con **múltiples niveles de suscripción** adaptados a las necesidades de diferentes empresas. Esto permitirá que empresas de menor tamaño puedan acceder a la plataforma sin comprometer su presupuesto, a la vez que se asegura el crecimiento a largo plazo a medida que la empresa crece.

#### d. Aprovechamiento de la digitalización en la logística
El sector de la logística está experimentando una transformación digital acelerada. **FuelTrack** se aprovechará de esta tendencia buscando la integración de la plataforma con otras soluciones logísticas (como los sistemas de gestión de vehículos o flotas). De esta forma podemos ofrecer una solución más completa y eficiente.

- **Táctica**: Colaborar con empresas de **gestión de flotas** para optimizar el proceso de asignación de vehículos, cisternas y choferes. También se considerará la posibilidad de integrar **sensores IoT** en los camiones de reparto para un control más preciso sobre el combustible transportado y la entrega.

#### e. Expansión hacia mercados internacionales
Si bien **FuelTrack** está inicialmente orientada a empresas locales, el modelo de negocio y la flexibilidad de la plataforma la hacen ideal para expandirse a **mercados internacionales**. Competidores como **Wialon** ya tienen presencia en mercados globales, pero su enfoque en empresas grandes y sus altos costos de implementación pueden ser una barrera para empresas de menor tamaño, limitando su alcance.

- **Táctica**: Iniciar la expansión en mercados emergentes donde la digitalización en la logística es una necesidad creciente. Esto incluirá la **localización de la plataforma** (idioma, moneda, regulaciones locales) para facilitar la adaptabilidad de los nuevos mercados.

## 2.2. Entrevistas.
### 2.2.1. Diseño de entrevistas.

Para comprender mejor a nuestros segmentos objetivo, se han definido dos entrevistas diferenciadas según el segmento objetivo: 
- Proveedores de combustible
- Empresas con contratos de suministro (clientes corporativos)

---
#### A. Proveedores de Combustible

**Preguntas:**

1. ¿Cómo gestionan actualmente los pedidos de empresas clientes?
2. ¿Usan algún sistema digital para registrar pedidos o es manual?
3. ¿Qué pasos se siguen desde que un cliente hace un pedido hasta que se entregue?
4. ¿Cómo controlan que lo despachado coincida con lo solicitado?
5. ¿Qué tipo de reportes requieren generar (volúmenes, facturación, entregas, etc.)?
6. ¿Tienen un sistema para validar el stock antes de preparar el despacho de un pedido?
7. ¿Cómo hacen el seguimiento de los pedidos? ¿Informan al cliente en tiempo real?
8. ¿Qué problemas suelen ocurrir en el proceso de atención de pedidos empresariales?
9. ¿Cómo se realiza la conciliación de pagos con los clientes?
10. ¿Estarían dispuestos a integrar su sistema actual con una plataforma SaaS que unifique y centralice estos procesos?


**Preguntas complementarias:**

- ¿Qué edad tiene?
- ¿Cuál es su nivel de experiencia en logística o ventas?
- ¿Qué tipo de dispositivo usa en el trabajo? (PC, tablet, celular)
- ¿Qué aplicaciones o herramientas digitales usa en su día a día?
- ¿Cómo describiría su nivel de habilidad con la tecnología?

---

#### B. Empresas Solicitantes

**Preguntas:**

1. ¿Cómo solicitan actualmente combustible a su proveedor?
2. ¿Utilizan un sistema propio o envían pedidos por correo, WhatsApp, etc.?
3. ¿Cómo verifican que lo entregado coincida con lo solicitado?
4. ¿Tienen problemas con entregas incompletas o fuera de tiempo?
5. ¿Con qué frecuencia necesitan reportes de consumo, entregas o pagos?
6. ¿Qué tan importante es para ustedes tener trazabilidad de cada entrega?
7. ¿Quiénes son los responsables de validar pedidos y autorizar pagos?
8. ¿Cómo gestionan las reprogramaciones o cancelaciones de pedidos?
9. ¿Qué herramientas utilizan para monitorear el consumo mensual?
10. ¿Qué mejoras desearían ver en el proceso actual?

**Preguntas complementarias:**

- ¿Qué edad tiene?
- ¿En qué distrito vive y trabaja?
- ¿Qué nivel de estudios tiene?
- ¿Qué dispositivos utiliza más frecuentemente en el trabajo?
- ¿Qué aplicaciones o plataformas usa para su gestión operativa?
- ¿Cuáles son sus principales frustraciones en el proceso actual?

---

<h3>2.2.2. Registro de entrevistas</h3>

<h4><u>Entrevista 1</u></h4>

<p><strong>Nombres:</strong> Carla<br>
<strong>Apellidos:</strong> Espejo<br>
<strong>Edad:</strong> 28<br>
<strong>Distrito:</strong> Lima</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista1.png" alt="entrevista_segmento1" /></p>

<p><strong>Inicio / Fin:</strong> 00:27 – 03:00<br>
<strong>Duración:</strong> 3:10<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u202213278_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202213278%5Fupc%5Fedu%5Fpe%2FDocuments%2F0418%2Emp4&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Edca00e68%2Db3ae%2D4379%2D8fd6%2D1446064f9809" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Carla, de 28 años y licenciada en Administración de Empresas, trabaja en Lima Metropolitana. En su empresa, enfrenta desafíos con la falta de automatización en los procesos, como la gestión manual de pedidos de combustibles que se hacen por correo o WhatsApp. Esto provoca confusión, retrasos y pérdida de información. La verificación de entregas también se hace manualmente, y monitorean el consumo con hojas de cálculo. Carla busca una plataforma que centralice los pedidos, permita seguimiento en tiempo real y automatice los reportes. Resaltó que mejorar estos procesos sería clave para su empresa.</p>

---

<h4><u>Entrevista 2</u></h4>

<p><strong>Nombres:</strong> Grover<br>
<strong>Apellidos:</strong> Manosalva<br>
<strong>Edad:</strong> 28<br>
<strong>Distrito:</strong> Lima</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista2.png" alt="entrevista_segmento1" /></p>

<p><strong>Inicio / Fin:</strong> 01:12 – 15:25<br>
<strong>Duración:</strong> 15:43<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u202310129_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202310129%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevista%20grover%20manosalva%2Emp4&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E60eca17f%2D505e%2D45a6%2D8680%2D9f3463341fbd" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Grover, de 28 años, trabaja en Cajamarca para una empresa extranjera del rubro de construcción y administración con operaciones en varias regiones del Perú. La compra de combustible se realiza directamente a Petroperú mediante la plataforma virtual de Osinergmin. El proceso inicia en el área de almacén, pasa por logística y se aprueba por la gerencia antes de generar la orden de compra, que se envía por correo o WhatsApp. El consumo se monitorea digitalmente con tablets que registran datos como horómetro, conductor y hora de abastecimiento. El área de equipos analiza esta información con fórmulas que alertan sobre consumos fuera del rango normal, lo cual ayuda a detectar posibles irregularidades. Grover sugiere como mejora que el sistema permita reprogramar fechas de carga sin necesidad de anular y generar nuevos pedidos. En su trabajo utiliza laptop, celular, teléfono corporativo y radios satelitales. Señaló que centralizar y flexibilizar estos procesos sería de gran ayuda para su empresa.</p>

---
<h4><u>Entrevista 3 </u></h4>

<p><strong>Nombres:</strong> Alfredo<br>
<strong>Apellidos:</strong> De Ure<br>
<strong>Edad:</strong> 25 años<br>
<strong>Distrito:</strong> Lima</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista3.png" alt="entrevista_segmento1" /></p>

<p><strong>Inicio / Fin:</strong> 00:12 – 15:25<br>
<strong>Duración:</strong> 6:35<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u202110373_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202110373%5Fupc%5Fedu%5Fpe%2FDocuments%2Fvideo1307550381%2Emp4&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E2f6a4453%2Db6c5%2D4961%2D8c5f%2D5dc0866d7117" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Alfredo trabaja en logística y utiliza principalmente computadora y celular. Su empresa solicita combustibles vía correos electrónicos, mensajes o llamadas, sin contar con un sistema digital propio. La verificación de entregas se hace mediante mediciones, aunque se presentan retrasos y entregas incompletas ocasionalmente. Los consumos se reportan de forma mensual y los resultados se compilan trimestralmente. La trazabilidad es un aspecto importante debido a requerimientos de auditoría.</p>

<p>Las validaciones de pedidos son realizadas por el jefe de área y el área de tesorería. Las reprogramaciones se gestionan a través de correos o llamadas. Utilizan medidores y un software para el control de consumos. Actualmente buscan automatizar los procesos para lograr mayor eficiencia operativa.</p>

---

<h4><u>Entrevista 4 </u></h4>

<p><strong>Nombres:</strong> Zahir<br>
<strong>Apellidos:</strong> Sanchez<br>
<strong>Edad:</strong> 25 años<br>
<strong>Distrito:</strong> Lima</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista4.png" alt="entrevista_segmento1" /></p>

<p><strong>Inicio / Fin:</strong> 00:14 – 05:28<br>
<strong>Duración:</strong> 5:35<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u201817507_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu201817507%5Fupc%5Fedu%5Fpe%2FDocuments%2Fentrevista%202%20open%20source%2020%2D04%2D2025%2Emp4&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E44981c48%2Db1d6%2D4ac7%2D8afd%2D0bdb857ded18" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Zahir trabaja registrando pedidos en Petromax. Los pedidos llegan primero por correo y luego se ingresan manualmente en su sistema interno (RPY). Controlan la entrega verificando volúmenes en planta y generan reportes diarios y mensuales de volúmenes y ventas. Validan el stock manualmente comunicándose con las plantas.</p>

<p>El seguimiento de pedidos se realiza por teléfono o WhatsApp. El principal problema que identifica es el riesgo de errores debido al registro manual. La conciliación de pagos es manejada por el área de cobranzas. Zahir manifestó estar dispuesto a adoptar una plataforma que unifique y automatice todo el proceso para reducir errores y mejorar la eficiencia.</p>

---

<h4><u>Entrevista 5 </u></h4>

<p><strong>Nombres:</strong> Patrick<br>
<strong>Apellidos:</strong> Chira<br>
<strong>Edad:</strong> 25 años<br>
<strong>Distrito:</strong> Piura</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista5.png" alt="entrevista_segmento1" /></p>

<p><strong>Duración:</strong> 13:14<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u202412591_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202412591%5Fupc%5Fedu%5Fpe%2FDocuments%2FV%C3%ADdeo%20sin%20t%C3%ADtulo%20%E2%80%90%20Hecho%20con%20Clipchamp%2Emp4&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E336e8a8d%2De640%2D4e6f%2Da835%2D40c4bc19e740&mode=View" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Patrick, de 25 años, trabaja desde hace un año en logística y maneja tecnología a nivel intermedio. Utiliza computadora, celular y tablet para gestionar pedidos de combustible de forma manual. Recibe solicitudes por correo o WhatsApp, verifica el stock en hojas de Excel y programa las entregas. Emite guías físicas y realiza la facturación en un plazo de 24 a 48 horas.</p>

<p>Utiliza herramientas como Excel, Google Drive, WhatsApp Business, SUNAT/Clave Sol y Google Maps. Entre los principales problemas que enfrenta se encuentran la falta de centralización del proceso, las demoras en la atención y los errores humanos. Señala que necesita una plataforma que centralice los pedidos, permita trazabilidad y agilice tanto la facturación como los reportes.</p>

---
<h4><u>Entrevista 6 </u></h4>

<p><strong>Nombres:</strong> Angie<br>
<strong>Apellidos:</strong> Santos<br>
<strong>Edad:</strong> 25 años<br>
<strong>Distrito:</strong> Piura</p>

<p><strong>Captura de la entrevista:</strong><br>
<img src="img/entrevista6.png" alt="entrevista_segmento1" /></p>

<p><strong>Inicio / Fin:</strong> 00:42 – 11:47<br>
<strong>Duración:</strong> 11:47<br>
<strong>URL de Entrevista:</strong> 
<a href="https://upcedupe-my.sharepoint.com/personal/u202412591_upc_edu_pe/_layouts/15/stream.aspx?id=%2Fpersonal%2Fu202412591%5Fupc%5Fedu%5Fpe%2FDocuments%2F2025%2D04%2D18%2023%2D46%2D00%2Emkv&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJTdHJlYW1XZWJBcHAiLCJyZWZlcnJhbFZpZXciOiJTaGFyZURpYWxvZy1MaW5rIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXcifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2Eb96a0d14%2Dc362%2D40ee%2D81e3%2Df385320344a2" target="_blank">Ver video</a></p>

<h5><strong>Resumen:</strong></h5>
<p>Angie, de 25 años y con un año de experiencia en logística, gestiona pedidos de combustible que recibe por WhatsApp, correo electrónico o formulario web. Registra los pedidos en Excel, verifica el stock mediante plantillas diarias, programa las rutas y notifica a los conductores. Utiliza GPS para seguimiento y emite factura electrónica en un plazo de 24 a 48 horas.</p>

<p>Entre los principales retos que enfrenta están los cambios de dirección de último minuto, el tráfico y los errores manuales. Para mitigar estos problemas, su empresa ha implementado confirmaciones 24 horas antes y sesiones de capacitación. Angie mostró interés en FuelTrack debido a su trazabilidad, geolocalización en tiempo real, firma digital, panel administrativo integrado y apps para choferes y administración. Incluso está dispuesta a participar en un piloto de la solución.</p>

    
---

<h3>2.2.3. Análisis de entrevistas</h3>

<h4><u>SEGMENTO 1: Empresas solicitantes de combustible</u></h4>

<h5>Características objetivas:</h5>
<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Variable</th>
      <th>Porcentaje</th>
      <th>Observaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Edad entre 30 y 45 años</td><td>100%</td><td>Todos los entrevistados tienen entre 33 y 45 años.</td></tr>
    <tr><td>Cargo relacionado a logística</td><td>100%</td><td>Los tres pertenecen a áreas de operaciones o logística.</td></tr>
    <tr><td>Usa computadora y celular</td><td>100%</td><td>Todos usan laptop/PC y móvil para sus actividades.</td></tr>
    <tr><td>Utiliza WhatsApp para coordinar</td><td>66%</td><td>2 de 3 lo usan como canal principal con el proveedor.</td></tr>
    <tr><td>Manejo de hojas Excel o Google</td><td>100%</td><td>Todos gestionan sus pedidos manualmente en planillas.</td></tr>
    <tr><td>Nivel medio de familiaridad digital</td><td>100%</td><td>Dominan software básico (Drive, correo, hojas de cálculo).</td></tr>
  </tbody>
</table>

<h5>Características subjetivas:</h5>
<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Variable</th>
      <th>Porcentaje</th>
      <th>Observaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Necesita trazabilidad del pedido</td><td>100%</td><td>Todos demandan claridad en el estado y avance del pedido.</td></tr>
    <tr><td>Frustración por depósitos no validados</td><td>66%</td><td>2 de 3 se quejan de retrasos debido a validación manual.</td></tr>
    <tr><td>Deseo de un sistema unificado</td><td>100%</td><td>Los 3 expresaron querer centralizar todo el proceso.</td></tr>
    <tr><td>Receptividad positiva a tecnología</td><td>100%</td><td>Todos están abiertos a soluciones digitales con buena UX.</td></tr>
  </tbody>
</table>

<hr>

<h4><u>SEGMENTO 2: Proveedores de combustible</u></h4>

<h5>Características objetivas:</h5>
<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Variable</th>
      <th>Porcentaje</th>
      <th>Observaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Edad entre 39 y 48 años</td><td>100%</td><td>Todos están en ese rango.</td></tr>
    <tr><td>Cargo en operaciones/logística</td><td>100%</td><td>Incluye jefes de planta, despacho o ventas.</td></tr>
    <tr><td>Utiliza laptop/PC y celular</td><td>100%</td><td>Equipamiento estándar en planta o administración.</td></tr>
    <tr><td>Nivel de digitalización medio</td><td>66%</td><td>2 de 3 usan sistemas propios o ERPs básicos.</td></tr>
    <tr><td>Gestión mediante correo y llamadas</td><td>100%</td><td>El proceso actual es altamente manual.</td></tr>
  </tbody>
</table>

<h5>Características subjetivas:</h5>
<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Variable</th>
      <th>Porcentaje</th>
      <th>Observaciones</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Problemas con conciliación bancaria</td><td>100%</td><td>Todos mencionan validación lenta de pagos como cuello de botella.</td></tr>
    <tr><td>Necesidad de validar stock antes de liberar</td><td>66%</td><td>2 de 3 destacaron esto como un punto crítico.</td></tr>
    <tr><td>Dificultades en la asignación de vehículos</td><td>66%</td><td>Errores de programación y disponibilidad afectan la entrega.</td></tr>
    <tr><td>Deseo de automatización de procesos</td><td>100%</td><td>Todos visualizan mejoras en eficiencia si se digitalizan etapas clave.</td></tr>
  </tbody>
</table>


## 2.3. Needfinding.
### 2.3.1. User Personas.

a. User Persona 1: Empresas solicitantes de combustible
![userpersona_segmento1](img/userpersona_segmento1.png)

b. User Persona 2: Proveedores de combustible
![userpersona_segmento2](img/userpersona_segmento2.png)

### 2.3.2. User Task Matrix.

| **Tarea**                                      | **David Miller – Frecuencia** | **David Miller – Importancia** | **Ana Pérez – Frecuencia** | **Ana Pérez – Importancia** |
|------------------------------------------------|-------------------------------|---------------------------------|-----------------------------|------------------------------|
| Revisar nivel de stock de combustible          | Alta | Alta | Baja | Baja |
| Realizar pedido de combustible                 | Media | Alta | Alta | Alta |
| Validar confirmación de pedido                 | Alta | Alta | Alta | Alta |
| Hacer seguimiento a la entrega                 | Alta | Alta | Alta | Alta |
| Supervisar descarga y recepción                | Media | Alta | Media | Media |
| Evaluar proceso post-servicio                  | Baja | Media | Alta | Alta |
| Gestionar atención al cliente                  | Media | Alta | Alta | Alta |
| Revisar encuestas o feedback                   | Baja | Media | Media | Alta |

### 2.3.3. User Journey Mapping.

En el caso del **solicitante**, el recorrido empieza con la generación de un pedido por correo o llamada, seguido por la validación manual del depósito, la espera de aprobación por parte del proveedor, la coordinación del despacho, y finalmente el registro manual de la entrega.

En el caso del **proveedor**, el flujo parte desde la recepción del pedido, luego incluye la verificación del estado de cuenta, la aprobación manual, la asignación de planta y vehículo, y en muchos casos, la reprogramación por problemas de disponibilidad.

a. User Persona 1: Empresas solicitantes de combustible
![userjourneymap_userpersona1](img/userjourneymap_userpersona1.png)

b. User Persona 2: Proveedores de combustible
![userjourneymap_userpersona2](img/userjourneymap_userpersona2.png)

### 2.3.4. Empathy Mapping.

![empathymap_segmento1](img/empathymap_segmento1.png)
![empathymap_segmento1](img/empathymap_segmento2.png)

### 2.3.5. As-is Scenario Mapping. 
### As-Is Scenario Mapping

| FASES | Comunicación | Solicitar pedido | Seguimiento | Entrega |
|-------|--------------|------------------|-------------|---------|
| **DOING** | Llamadas, correos, WhatsApp sin orden. | El solicitante explica los datos del pedido a mano. | Se hacen llamadas para preguntar por el estado. | Se confirma por llamada o mensaje. |
| **THINKING** | "¿Habrán recibido mi mensaje?" | "¿Me habrán entendido bien?" | "¿Dónde estará nuestro pedido?" | "¿Ya habrán llegado?" |
| **FEELING** | Frustración, desorganización. | Incertidumbre, falta de confianza. | Ansiedad, impaciencia. | Duda, estrés. |

## 2.4. Ubiquitous Language. 

| Término | Definición | Segmentos relacionados |
|---------|------------|------------------------|
| **Requester (Solicitante)** | Usuario representante de una empresa requiere abastecimiento de combustible | Solicitante |
| **Supplier (Proveedor)** | Empresa que ofrece combustibles al por mayor y compite mediante precios, descuentos y promociones. | Proveedor |
| **Fuel (Combustible)** | Recurso energético que es ofertado por los proveedores. Ejemplos: gasohol, diésel, GNV. | Solicitante, Proveedor |
| **Plant (Planta)** | Punto de distribución del combustible perteneciente a al proveedor. | Solicitante, Proveedor |
| **Price per gallon (Precio por galón)** | Valor económico que el proveedor establece por cada galón de combustible. Puede variar según planta, tipo de combustible, etc. | Solicitante, Proveedor |
| **Discount (Descuento)** | Reducción aplicada sobre el precio ofrecido, ya sea por volumen, fidelización u otras condicioens. | Solicitante, Proveedor |
| **Quotation (Cotización)** | Propuesta formal que un proveedor genera detallando precios, productos, entre otras condiciones | Solicitante, Proveedor |
| **Price Table (Tabla de precios)** | Grilla o tabla que muestra los precios ofrecidos por planta, proveedor y tipo de combustible. | Solicitante |
| **Negotiation (Negociación)**   | Intercambio de condiciones entre solicitante y proveedor para alcanzar un acuerdo favorable para ambas partes. | Solicitante, Proveedor |
| **Consumption Volume (Volumen de consumo)** | Cantidad de combustible estimada que una empresa solicita regularmente en un periodo determinado. | Solicitante |
| **Purchase History (Historial de compras)** | Registro de cotizaciones y compras o pedidos previos hechos por el solicitante dentro del sistema. | Solicitante |