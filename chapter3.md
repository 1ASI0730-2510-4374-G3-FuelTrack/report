# Capitulo III: Requirements Specifications
<h3>3.1 To-Be Scenario Mapping</h3>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>FASES</th>
      <th>Comunicación</th>
      <th>Solicitar pedido</th>
      <th>Seguimiento</th>
      <th>Entrega</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>DOING</strong></td>
      <td>Utiliza la plataforma centralizada FuelTracks, con historial de comunicación y notificaciones automáticas.</td>
      <td>Completa un formulario estructurado directamente desde la web o app.</td>
      <td>Revisa el panel de seguimiento con estado del pedido en tiempo real.</td>
      <td>Recibe una confirmación automática con hora estimada y firma digital.</td>
    </tr>
    <tr>
      <td><strong>THINKING</strong></td>
      <td>"Puedo revisar todos mis pedidos desde un solo lugar."</td>
      <td>"Todo quedó registrado sin ningún error."</td>
      <td>"Puedo ver exactamente en qué etapa está mi pedido y cuánto falta para que pueda recibirlo."</td>
      <td>"Recibí el pedido tal como estaba programado."</td>
    </tr>
    <tr>
      <td><strong>FEELING</strong></td>
      <td>Tranquilidad, control.</td>
      <td>Confianza, seguridad.</td>
      <td>Calma, claridad.</td>
      <td>Satisfacción, alivio.</td>
    </tr>
  </tbody>
</table>


---

<h3>3.2 User Stories</h3>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Epic ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de aceptación</th>
      <th>Relacionado con (Epic ID)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>EP01</td>
      <td>Gestión de pedidos de combustible de solicitante</td>
      <td>Como usuario solicitante de combustible, quiero poder registrar mis pedidos fácilmente y con la capacidad de establecer parámetros específicos para evitar errores en la comunicación y recibir lo que necesito.</td>
      <td><strong>Escenario 1</strong>: Registro de pedido exitoso. En la plataforma, debería ver una sección en la plataforma para realizar nuevos pedidos, donde encuentre un formulario en el que pueda especificar lo que necesito y posteriormente registrar la orden. <br/> <strong>Escenario 2</strong>: Visualización de historial de pedidos. Debería ser capaz de visualizar una sección que muestre todos mis pedidos anteriores. <br/> <strong>Escenario 3</strong>: Edición antes de la confirmación. Antes de que los pedidos sean confirmados por los proovedores, debería tener la posibilidad de hacer ediciones a este o incluso poder cancelarlo.</td>
      <td>-</td>
    </tr>
    <tr>
      <td>EP02</td>
      <td>Gestión de pedidos recibidos por el proovedoor</td>
      <td>Como usuario proovedor de combustible, quiero poder revisar los pedidos realizados por mis clientes, actualizar el estado de cada uno y dar actualizaciones en tiempo real a mis clientes.</td>
      <td><strong>Escenario 1</strong>: Visualización de pedidos entrantes. Dado que haya pedidos activos, Cuando el proveedor acceda a su panel, Entonces debería poder ver una lista de pedidos con detalles clave (cliente, ubicación, volumen, estado). <br/> <strong>Escenario 2</strong>: Actualización de estado del pedido.Dado que un pedido esté en curso,Cuando el proveedor actualice su estado (confirmado, en ruta, entregado),Entonces el sistema deberá reflejar el cambio en tiempo real. <br/> <strong>Escenario 3</strong>: Notificación a los clientes. Dado que el proveedor realice un cambio o actualización a un pedido, Cuando el cliente esté en la plataforma, entonces deberá ver una notificación con información de los cambios ocurridos.</td>
      <td>-</td>
    </tr>
    <tr>
      <td>EP03</td>
      <td>Gestión de seguridad y acceso</td>
      <td>Como usuario de ambos segmentos de la plataforma, quiero que mis datos estén protegidos y acceder solo mediante autenticación segura, para garantizar la privacidad y evitar accesos no autorizados.</td>
      <td><strong>Escenario 1</strong>: Inicio de sesión seguro. Dado que el usuario tenga una cuenta, Cuando intente iniciar sesión con correo y contraseña, Entonces el sistema debe validar las credenciales y otorgar acceso solo si son correctas, evitando revelar información en caso de error. <br/> <strong>Escenario 2</strong>: Control de accesos según rol. Dado que un usuario (cliente o proveedor) haya iniciado sesión,Cuando intente acceder a secciones específicas de la plataforma, Entonces solo deberá poder ver y operar dentro de las funcionalidades permitidas por su tipo de cuenta. <br/> <strong>Escenario 3</strong>: Autenticación multifactor para operaciones. Dado que un cliente esté realizando un pedido,Cuando intente enviarlo o confirmarlo,Entonces el sistema deberá activar un segundo paso de verificación (código temporal o notificación) antes de procesar la acción..</td>
      <td>-</td>
    </tr>
    <tr>
      <td>EP04</td>
      <td>Landing Page informativa y funcional</td>
      <td>Como parte de la solución, quiero ofrecer una landing page que muestre los beneficios y funcionalidades de FuelTrack, para captar el interés de potenciales usuarios.</td>
      <td><strong>Escenario 1</strong>: Visualización pública. Cuando alguien acceda al dominio principal sin estar autenticado, el sistema debe mostrar la landing page con secciones informativas, beneficios del sistema, segmentos objetivo y llamadas a la acción hacia login/registro. <br/> <strong>Escenario 2</strong>: Redirección según interés. Al hacer clic en 'Quiero registrarme', debe llevar al formulario correspondiente según el segmento.</td>
      <td>-</td>
    </tr>
  </tbody>
</table>


<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>User Story ID</th>
      <th>Título</th>
      <th>Descripción</th>
      <th>Criterios de aceptación</th>
      <th>Relacionado con (Epic ID)</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>US01</td>
      <td>Crear nuevo pedido</td>
      <td>Como usuario de una empresa solicitante, quiero poder registrar un pedido directamente desde la plataforma agilizar el proceso y evitar llamadas.</td>
      <td>Dado que el usuario ingrese todos los campos requeridos, Cuando envíe el pedido, Entonces el sistema deberá procesarlo, asignar un ID único y enviarlo a los proovedores para que confirmen la orden.</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US02</td>
      <td>Consultar historial de pedidos</td>
      <td>Como solicitante, quiero poder consultar mi historial de pedidos anteriores, y poder ver cada uno con información detallada. Además, debo ser capaz de filtrar y ordenar el historial según características específicas de los pedidos.</td>
      <td>Dado que el usuario acceda a la sección de seguimiento,Cuando seleccione un pedido,Entonces podrá ver si fue recibido, confirmado, en ruta o entregado.</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US03</td>
      <td>Editar pedidos</td>
      <td>Como solicitante, quiero tener la posibilidad de editar parámetros, como el monto o dirección de entrega, de mis pedidos siempre y cuando estos todavía no hayan sido confirmados por el rpoovedor</td>
      <td>Dado que el usuario acceda a la sección de pedidos activo, Cuando seleccione un pedido que se encuentra sin confirmar ,Entonces podrá editar los parámetros del pedido.</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US05</td>
      <td>Actualización de un pedido</td>
      <td>Como proveedor de combustible, quiero poder actualizar el estado e información de los pedidos en tiempo real, para mantener a mis clientes informados y organizar mejor mis entregas.</td>
      <td>Dado que existan pedidos activos para el proveedor, Cuando el proveedor los seleccione,Entonces el sistema deberá darle la posibilidad de hacerle cambios o darle actualizaciones.</td>
      <td>-</td>
    </tr>
    <tr>
      <td>US06</td>
      <td>Notificaciones a clientes sobre cambios</td>
      <td>Como proovedor, quiero que mis clientes reciban notificaciones automáticas cuando actualizo un pedido, para que estén al tanto del progreso sin tener que llamarlos.</td>
      <td>Dado que se modifique el estado o datos del pedido, Cuando se actualice a "confirmado", "en ruta" o "entregado", Entonces el sistema debe enviar una notificación push, correo o WhatsApp al cliente.</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US07</td>
      <td>Cancelación o rechazo de pedidos</td>
      <td>Como proveedor de combustible, quiero poder rechazar o cancelar un pedido y enviar un mensaje al cliente explicando los motivos, para mantener una comunicación clara y evitar confusiones.</td>
      <td>Dado que el proveedor no pueda atender un pedido,Cuando seleccione la opción de cancelar o rechazar,Entonces el sistema deberá solicitarle ingresar un mensaje explicando el motivo y notificar al cliente con dicha información.</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US08</td>
      <td>Inicio de sesión</td>
      <td>Como usuario registrado, quiero iniciar sesión con mi correo y contraseña, para acceder a mi cuenta de forma segura.</td>
      <td>Dado que el usuario tenga una cuenta, Cuando intente iniciar sesión,Entonces el sistema deberá validar sus credenciales y permitir el acceso solo si son correctas.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US09</td>
      <td>Registro de cuenta nueva</td>
      <td>Como visitante, Quiero crear una cuenta con correo, contraseña y rol (cliente o proveedor), Para acceder y comenzar a utilizar la plataforma.</td>
      <td>Dado que el usuario complete todos los campos requeridos, Cuando presione “Crear cuenta”, Entonces la cuenta deberá crearse correctamente y redirigirlo a su panel.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US10</td>
      <td>Recuperación de contraseña</td>
      <td>Como usuario, Quiero tener la posibilidad de recuperar mi contraseña mediante correo electrónico, Para no perder el acceso a mi cuenta en caso la olvide.</td>
      <td>Dado que el usuario no recuerde su contraseña, Cuando seleccione “¿Olvidaste tu contraseña?”,Entonces deberá recibir un correo con un enlace para restablecerla.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US11</td>
      <td>Acceso restringido por roles</td>
      <td>Como administrador de la plataforma, Quiero que los usuarios solo accedan a las secciones según su tipo de cuenta, Para evitar errores en el sistema</td>
      <td>Dado que un usuario acceda a la plataforma, Cuando vea las secciones que tiene disponible, Entonces verá únicamente las que son correspondientes a su rol.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US12</td>
      <td>Autenticación MFA para realizar pedidos</td>
      <td>Como empresa solicitante, Quiero que se me solicite una autenticación multifactor al momento de realizar un pedido, Para asegurar que solo personal autorizado pueda emitir órdenes de compra</td>
      <td>Dado que el cliente quiera registrar un pedido, Cuando complete los datos del formulario de registro, Entonces deberá recibir un código de autenticación y solo podrá finalizar el pedido tras ingresarlo correctamente.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US13</td>
      <td>Visualización del landing page</td>
      <td>Como usuario de la plataforma, quiero que el sistema muestre un landing page informativo para que los interesados conozcan los beneficios antes de registrarse.</td>
      <td>Dado que alguien acceda a la URL principal, Cuando no esté autenticado, Entonces deberá visualizar el landing page con secciones informativas y botones hacia login o registro.</td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>TS01</td>
      <td>Implementar endpoint REST para pedidos</td>
      <td>Como desarrollador, quiero implementar un endpoint RESTful para registrar pedidos, para que la aplicación frontend pueda enviar solicitudes válidas al backend.</td>
      <td>Dado que se realice una solicitud POST con datos válidos, Cuando se procese en el backend, Entonces deberá guardarse el pedido en la base de datos y devolver un código 201 con ID.</td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>TS02</td>
      <td>Servicio de autenticación y token</td>
      <td>Como desarrollador, quiero implementar un servicio de autenticación con generación de tokens, para proteger las rutas privadas de la plataforma.</td>
      <td>Dado que un usuario inicie sesión, Cuando las credenciales sean válidas, Entonces el sistema deberá generar un token JWT para acceso a recursos protegidos.</td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>TS03</td>
      <td>Envío de notificaciones por cambios de estado</td>
      <td>Como desarrollador, quiero implementar un servicio que envíe notificaciones automáticas cuando un pedido cambie de estado, para mantener informados a los usuarios.</td>
      <td>Dado que el estado de un pedido sea actualizado, Cuando se complete la acción, Entonces deberá enviarse una notificación por correo o WhatsApp al usuario correspondiente.</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>TS04</td>
      <td>Registro y validación de ubicación GPS</td>
      <td>Como desarrollador, quiero permitir que los pedidos en ruta envíen coordenadas GPS, para poder visualizar la trazabilidad del transporte en tiempo real.</td>
      <td>Dado que un conductor envíe su ubicación, Cuando el backend reciba las coordenadas, Entonces deberán almacenarse y estar disponibles para visualización en el frontend.</td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US14</td>
      <td>Ver sección Home</td>
      <td>Como visitante (proveedor), quiero ver una sección de inicio que resuma el valor de FuelTrack para comprender rápidamente el objetivo del sistema.</td>
      <td>
        Escenario 1: Visualización de resumen del sistema.<br/>
        Escenario 2: Acceso a call to action desde Home.
      </td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US15</td>
      <td>Ver sección About Us</td>
      <td>Como visitante de ambos segmentos, quiero conocer quiénes están detrás de FuelTrack para confiar en el sistema.</td>
      <td>
        Escenario 1: Información visible del equipo.<br/>
        Escenario 2: Ver valores o misión.
      </td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US16</td>
      <td>Ver sección How it works?</td>
      <td>Como visitante de ambos segmentos, quiero entender cómo funciona FuelTrack paso a paso para evaluar si se ajusta a mis necesidades.</td>
      <td>
        Escenario 1: Comprensión del flujo de pedidos.<br/>
        Escenario 2: Interacción clara entre usuarios.
      </td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US17</td>
      <td>Enviar mensaje de contacto</td>
      <td>Como visitante de ambos segmentos, quiero enviar un mensaje desde Contact Us para solicitar más información.</td>
      <td>
        Escenario 1: Envío exitoso de mensaje.<br/>
        Escenario 2: Validación de campos obligatorios.<br/>
        Escenario 3: Confirmación visual del envío.
      </td>
      <td>EP04</td>
    </tr>
    <tr>
      <td>US18</td>
      <td>Aprobar pedido</td>
      <td>Como proveedor, quiero aceptar según el stock disponible para evitar conflictos de distribución.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Aprobación de pedido con stock disponible</strong>
            <ul>
              <li>Dado que el proveedor tiene stock suficiente,</li>
              <li>Cuando aprueba el pedido,</li>
              <li>Entonces el estado cambia a “Aprobado”.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Envío de motivo</strong>
            <ul>
              <li>Dado que el proveedor decide no aprobar un pedido por un periodo de tiempo,</li>
              <li>Cuando revise los pedidos,</li>
              <li>Entonces el sistema solicita ingresar una razón.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US19</td>
      <td>Marcar pedido como despachado</td>
      <td>Como proveedor, quiero marcar cuándo un pedido sale a entrega para notificar al cliente.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Despacho exitoso de un pedido</strong>
            <ul>
              <li>Dado que el proveedor tiene un pedido aprobado,</li>
              <li>Cuando marca el pedido como despachado,</li>
              <li>Entonces el estado cambia a “Despachado”.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Restricción de despacho sin aprobación previa</strong>
            <ul>
              <li>Dado que el proveedor intenta despachar un pedido sin aprobación,</li>
              <li>Cuando ejecuta la acción,</li>
              <li>Entonces el sistema impide el cambio de estado y muestra un mensaje.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US20</td>
      <td>Cerrar pedido</td>
      <td>Como proveedor, quiero cerrar el pedido cuando el cliente confirme la entrega para finalizar el proceso.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Cierre correcto del pedido tras confirmación</strong>
            <ul>
              <li>Dado que el solicitante ya confirmó la entrega,</li>
              <li>Cuando el proveedor cierra el pedido,</li>
              <li>Entonces este no puede modificarse más.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Intento de cierre sin confirmación previa</strong>
            <ul>
              <li>Dado que el proveedor intenta cerrar el pedido,</li>
              <li>Cuando el solicitante aún no ha confirmado la entrega,</li>
              <li>Entonces el sistema impide esta acción.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US21</td>
      <td>Generar reporte de ventas</td>
      <td>Como proveedor, quiero generar reportes de ventas para tener registro de operaciones realizadas.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Generación de reporte con datos disponibles</strong>
            <ul>
              <li>Dado que el proveedor selecciona un rango de fechas válido,</li>
              <li>Cuando solicita el reporte,</li>
              <li>Entonces se genera un archivo con los datos de ventas.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Generación sin datos en el rango</strong>
            <ul>
              <li>Dado que el proveedor selecciona un rango sin ventas,</li>
              <li>Cuando solicita el reporte,</li>
              <li>Entonces el sistema informa que no hay resultados.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Descarga del archivo generado</strong>
            <ul>
              <li>Dado que el reporte se genera correctamente,</li>
              <li>Cuando finaliza el proceso,</li>
              <li>Entonces el proveedor puede descargar el archivo.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US22</td>
      <td>Ver resumen de pedidos (Solicitante)</td>
      <td>Como solicitante, quiero ver un resumen de mis pedidos para identificar cuántos están en proceso o completados.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Visualización de resumen con datos disponibles</strong>
            <ul>
              <li>Dado que el solicitante tiene pedidos registrados,</li>
              <li>Cuando accede a su dashboard,</li>
              <li>Entonces visualiza los KPIs por estado: pendientes, aprobados, despachados, finalizados y rechazados.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Sin pedidos registrados</strong>
            <ul>
              <li>Dado que el solicitante no tiene pedidos,</li>
              <li>Cuando accede al dashboard,</li>
              <li>Entonces ve un mensaje informando “No hay pedidos registrados”.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Error al cargar datos del resumen</strong>
            <ul>
              <li>Dado que el solicitante accede al dashboard,</li>
              <li>Cuando ocurre un error de carga,</li>
              <li>Entonces el sistema muestra un mensaje e intenta recargar los datos automáticamente.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US23</td>
      <td>Ver resumen de pedidos (Proveedor)</td>
      <td>Como proveedor, quiero ver un resumen de pedidos gestionados y pendientes para organizar a los clientes.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Visualización de KPIs con datos</strong>
            <ul>
              <li>Dado que el proveedor tiene pedidos registrados,</li>
              <li>Cuando accede a su dashboard,</li>
              <li>Entonces ve KPIs de pedidos: pendientes, aprobados, rechazados, despachados y finalizados.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Sin datos registrados</strong>
            <ul>
              <li>Dado que no hay pedidos registrados,</li>
              <li>Cuando se carga el dashboard,</li>
              <li>Entonces los KPIs se muestran con valor cero y un mensaje informativo.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Fallo en la carga del resumen</strong>
            <ul>
              <li>Dado que el proveedor accede al dashboard,</li>
              <li>Cuando hay un error de conexión,</li>
              <li>Entonces se muestra una alerta con opción para reintentar.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>TS05</td>
      <td>Endpoint: Login</td>
      <td>Como developer, quiero un endpoint para autenticar usuarios.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Autenticación exitosa</strong>
            <ul>
              <li>Dado que el developer incluye credenciales válidas en el request,</li>
              <li>Cuando lo envía al endpoint de autenticación,</li>
              <li>Entonces recibe un token JWT y un status 200 como respuesta.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Credenciales inválidas</strong>
            <ul>
              <li>Dado que el developer incluye credenciales incorrectas en el request,</li>
              <li>Cuando se procesa la solicitud,</li>
              <li>Entonces se retorna status 401 con un mensaje de error.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Error interno del servidor</strong>
            <ul>
              <li>Dado que el developer realiza un request y ocurre un problema en el backend,</li>
              <li>Cuando se procesa la autenticación,</li>
              <li>Entonces se retorna status 500 con un mensaje genérico de error.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>TS06</td>
      <td>Endpoint: Recuperar contraseña</td>
      <td>Como developer, quiero un endpoint para que permita enviar correo de recuperación.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Solicitud válida</strong>
            <ul>
              <li>Dado que el developer envía un request con un correo que existe en la base de datos,</li>
              <li>Cuando el request llega al endpoint de recuperación,</li>
              <li>Entonces el sistema genera un token y envía el correo de recuperación.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Correo inexistente</strong>
            <ul>
              <li>Dado que el developer envía un request con un correo no registrado,</li>
              <li>Cuando se procesa la solicitud,</li>
              <li>Entonces se retorna status 404 y no se envía ningún correo.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Error en el envío del correo</strong>
            <ul>
              <li>Dado que el developer ejecuta la acción y ocurre un fallo en el servicio de correo,</li>
              <li>Cuando se intenta enviar el mensaje,</li>
              <li>Entonces se retorna status 500 y se registra el error en los logs del servidor.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>TS07</td>
      <td>Endpoint: Logout</td>
      <td>Como developer, quiero un endpoint para cerrar sesión.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Logout exitoso</strong>
            <ul>
              <li>Dado que el developer envía un token de sesión válido,</li>
              <li>Cuando llama al endpoint de logout,</li>
              <li>Entonces la sesión se invalida y se retorna status 200.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Token inválido o expirado</strong>
            <ul>
              <li>Dado que el developer incluye un token no válido o expirado,</li>
              <li>Cuando se llama al endpoint de logout,</li>
              <li>Entonces se retorna status 401 y no se realiza ninguna acción.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Falla del servidor</strong>
            <ul>
              <li>Dado que el developer realiza un request y ocurre un error interno en el servidor,</li>
              <li>Cuando se procesa el logout,</li>
              <li>Entonces se retorna status 500 con un mensaje genérico.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US24</td>
      <td>Asignar vehículo a pedido</td>
      <td>Como proveedor, quiero asignar un vehículo a un pedido aprobado para organizar la logística.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Asignación válida</strong>
            <ul>
              <li>Dado que el proveedor tiene un pedido aprobado y un vehículo libre disponible,</li>
              <li>Cuando selecciona el vehículo para asignarlo,</li>
              <li>Entonces queda asignado correctamente al pedido.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Vehículo ocupado</strong>
            <ul>
              <li>Dado que el proveedor intenta asignar un vehículo que ya está ocupado,</li>
              <li>Cuando realiza la acción,</li>
              <li>Entonces el sistema muestra un mensaje indicando que el vehículo no está disponible.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Falla durante la asignación</strong>
            <ul>
              <li>Dado que el proveedor intenta asignar un vehículo y ocurre un error en el backend,</li>
              <li>Cuando se ejecuta la asignación,</li>
              <li>Entonces se muestra un mensaje de error y no se vincula ningún vehículo.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US25</td>
      <td>Asignar conductor a pedido</td>
      <td>Como proveedor, quiero asignar un conductor para completar la información de despacho.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Conductor disponible</strong>
            <ul>
              <li>Dado que el proveedor tiene un pedido con vehículo asignado y el conductor está libre,</li>
              <li>Cuando selecciona al conductor,</li>
              <li>Entonces este se vincula correctamente al pedido.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Conductor ya asignado en misma franja horaria</strong>
            <ul>
              <li>Dado que el conductor está asignado a otro pedido en el mismo horario,</li>
              <li>Cuando se intenta asignarlo,</li>
              <li>Entonces el sistema bloquea la acción y muestra un mensaje de conflicto.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Error al guardar</strong>
            <ul>
              <li>Dado que el proveedor intenta guardar la asignación y ocurre una falla técnica,</li>
              <li>Cuando realiza la acción,</li>
              <li>Entonces se muestra un mensaje de error y no se realiza el vínculo.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US26</td>
      <td>Validar disponibilidad de transporte</td>
      <td>Como proveedor, quiero saber qué vehículos están disponibles antes de asignarlos para vincularlos correctamente.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Vehículo no disponible por superposición</strong>
            <ul>
              <li>Dado que el proveedor visualiza el listado de vehículos,</li>
              <li>Cuando un vehículo está asignado a otro pedido para la misma fecha y hora estimada,</li>
              <li>Entonces el sistema lo muestra como no disponible.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Vehículo disponible</strong>
            <ul>
              <li>Dado que el proveedor visualiza un vehículo sin conflictos de agenda,</li>
              <li>Cuando se carga el listado de vehículos,</li>
              <li>Entonces dicho vehículo se muestra como seleccionable.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Conflicto en tiempo real</strong>
            <ul>
              <li>Dado que el proveedor intenta seleccionar un vehículo que fue asignado recientemente por otro usuario,</li>
              <li>Cuando realiza la acción,</li>
              <li>Entonces el sistema bloquea la selección y muestra un mensaje de actualización.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US27</td>
      <td>Ver perfil de usuario</td>
      <td>Como usuario registrado, quiero ver mis datos de perfil para revisar mi información registrada.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Visualización exitosa del perfil</strong>
            <ul>
              <li>Dado que el usuario tiene sesión activa,</li>
              <li>Cuando accede a su perfil,</li>
              <li>Entonces ve su nombre, correo y rol.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Error en la carga de datos</strong>
            <ul>
              <li>Dado que el usuario accede a su perfil y ocurre un error al obtener los datos,</li>
              <li>Cuando se carga la vista,</li>
              <li>Entonces se muestra un mensaje de error y se sugiere reintentar.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Restricción de datos de otros usuarios</strong>
            <ul>
              <li>Dado que el usuario tiene sesión activa,</li>
              <li>Cuando intenta ver otro perfil,</li>
              <li>Entonces el sistema restringe el acceso y muestra su propia información.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US28</td>
      <td>Editar datos de perfil</td>
      <td>Como usuario registrado, quiero editar mis datos para mantener mi información actualizada.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Edición y guardado exitoso</strong>
            <ul>
              <li>Dado que el usuario modifica uno o más campos del formulario,</li>
              <li>Cuando la información ingresada es válida,</li>
              <li>Entonces el sistema guarda los cambios correctamente.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Campo obligatorio vacío</strong>
            <ul>
              <li>Dado que el usuario deja un campo obligatorio vacío,</li>
              <li>Cuando intenta guardar,</li>
              <li>Entonces el sistema muestra un mensaje de validación indicando el campo requerido.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Error del servidor al guardar</strong>
            <ul>
              <li>Dado que el usuario intenta guardar y ocurre un fallo en el servidor,</li>
              <li>Cuando se realiza la acción,</li>
              <li>Entonces se muestra un mensaje de error y los datos ingresados permanecen visibles.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US29</td>
      <td>Buscar pedido por código</td>
      <td>Como usuario de ambos segmentos, quiero buscar un pedido específico por su código para encontrarlo rápidamente.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Ingresar a la búsqueda</strong>
            <ul>
              <li>Dado que el usuario presione el botón de filtrar,</li>
              <li>Cuando ingrese la opción del código en las grillas,</li>
              <li>Entonces podrá buscar su pedido según su código.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Pedido encontrado</strong>
            <ul>
              <li>Dado que el usuario escribe un código válido,</li>
              <li>Cuando existe un pedido con ese código,</li>
              <li>Entonces se muestra el resultado correspondiente.</li>
            </ul>
          </li>
          <li><strong>Escenario 3: Pedido no encontrado</strong>
            <ul>
              <li>Dado que el usuario digita un código no correspondiente a ningún pedido,</li>
              <li>Cuando finaliza la búsqueda,</li>
              <li>Entonces el sistema muestra un mensaje de que no hay coincidencias.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US30</td>
      <td>Filtrar pedidos por estado</td>
      <td>Como usuario de ambos segmentos, quiero filtrar mis pedidos por estado (pendiente, aprobado, entregado) para facilitar la revisión.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Aplicar filtro correctamente</strong>
            <ul>
              <li>Dado que el usuario selecciona un estado,</li>
              <li>Cuando se aplica el filtro,</li>
              <li>Entonces solo se muestran los pedidos con ese estado.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: No hay pedidos en ese estado</strong>
            <ul>
              <li>Dado que el usuario selecciona un estado que no tiene coincidencias,</li>
              <li>Cuando ejecuta el filtro,</li>
              <li>Entonces se muestra un mensaje indicando que no hay pedidos para ese estado.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP03</td>
    </tr>
    <tr>
      <td>US31</td>
      <td>Recibir notificación de aprobación</td>
      <td>Como solicitante, quiero recibir una notificación cuando un pedido sea aprobado o rechazado para estar informado.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Visualización de notificación</strong>
            <ul>
              <li>Dado que el proveedor cambia el estado del pedido,</li>
              <li>Cuando el solicitante inicia sesión,</li>
              <li>Entonces recibe la notificación del evento en la página y en las notificaciones.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Pedido actualizado desde otra sesión</strong>
            <ul>
              <li>Dado que el solicitante aún no ha leído la notificación,</li>
              <li>Cuando actualiza la interfaz,</li>
              <li>Entonces la notificación se mantiene visible hasta que sea marcada como leída.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US32</td>
      <td>Notificación de pedido despachado</td>
      <td>Como solicitante, quiero recibir una notificación cuando un pedido haya sido despachado para estar informado.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Pedido marcado como despachado</strong>
            <ul>
              <li>Dado que el proveedor marca el pedido como despachado,</li>
              <li>Cuando el solicitante consulta su cuenta,</li>
              <li>Entonces recibirá la notificación correspondiente en la página como en las notificaciones.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Visualización posterior del evento</strong>
            <ul>
              <li>Dado que el pedido fue despachado anteriormente,</li>
              <li>Cuando el solicitante accede en otro momento,</li>
              <li>Entonces la notificación sigue disponible hasta ser archivada o leída.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US33</td>
      <td>Ver listado de empresas</td>
      <td>Como proveedor, quiero ver una lista de empresas solicitantes para identificar a mis clientes frecuentes.</td>
      <td>
        <ul>
          <li><strong>Escenario 1: Visualización del listado</strong>
            <ul>
              <li>Dado que el proveedor accede al módulo de empresas,</li>
              <li>Cuando se carga el listado,</li>
              <li>Entonces se muestran nombre, pedidos activos y total histórico por empresa.</li>
            </ul>
          </li>
          <li><strong>Escenario 2: Lista vacía o sin datos</strong>
            <ul>
              <li>Dado que el proveedor accede al módulo y no hay empresas registradas,</li>
              <li>Cuando se carga la vista,</li>
              <li>Entonces se muestra un mensaje indicando que no hay empresas disponibles.</li>
            </ul>
          </li>
        </ul>
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US34</td>
      <td>Ver detalles de empresa</td>
      <td>Como proveedor, quiero ver información detallada de una empresa solicitante para analizar su historial de pedidos.</td>
      <td>
        Dado que el proveedor selecciona una empresa, Cuando se carga el detalle, Entonces visualiza pedidos realizados, cantidades solicitadas y fechas. Escenario 2: Dado que el proveedor selecciona una empresa que aún no ha realizado pedidos, Cuando se accede a su perfil, Entonces se muestra un mensaje indicando que no hay historial disponible.
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US35</td>
      <td>Ver gráfico de consumo (Solicitante)</td>
      <td>Como solicitante, quiero ver un gráfico de mi consumo mensual para tener control sobre el uso del combustible.</td>
      <td>
        Escenario 1: Dado que el solicitante ha realizado pedidos,Cuando accede al módulo de reportes, Entonces se visualiza un gráfico con galones consumidos por mes. Escenario 2: Dado que el solicitante no ha hecho pedidos aún, Cuando accede al gráfico, Entonces se muestra un mensaje de que no hay datos suficientes.
      </td>
      <td>EP01</td>
    </tr>
    <tr>
      <td>US36</td>
      <td>Ver gráfico de ventas (Proveedor)</td>
      <td>Como proveedor, quiero ver un gráfico de ventas por mes para monitorear el rendimiento del negocio.</td>
      <td>
        Dado que el proveedor ha despachado pedidos, Cuando accede al módulo de reportes, Entonces se visualiza un gráfico con las ventas mensuales totales. Escenario 2: Dado que el proveedor no ha realizado ventas aún, Cuando accede al gráfico, Entonces se muestra un mensaje de que no hay datos suficientes.
      </td>
      <td>EP02</td>
    </tr>
    <tr>
      <td>US37</td>
      <td>Descargar reporte PDF</td>
      <td>Como usuario de ambos segmentos, quiero descargar un resumen de pedidos o ventas en formato PDF para archivarlo o compartirlo.</td>
      <td>
        Escenario 1: Dado que el usuario hace clic en "Descargar", Cuando hay datos en el periodo seleccionado, Entonces se genera un archivo PDF descargable. Escenario 2: Dado que el usuario no tiene registros en el periodo seleccionado, Cuando se solicita la descarga, Entonces el sistema notifica que no hay contenido para exportar. Escenario 3: Dado que el usuario intenta descargar el archivo y ocurre un error en el backend al generar el PDF, Cuando hace clic en el botón de descargar, Entonces se muestra un mensaje de error sin afectar la sesión.
      </td>
      <td>-</td>
    </tr>
  </tbody>
</table>

## 3.3 Impact Mapping
![IM](img/Impact-Map.png)

<h3>3.4 Product Backlog</h3>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>#Orden</th>
      <th>ID</th>
      <th>User Story</th>
      <th>Story Points</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>01</td><td>US-01</td><td>Crear nuevo pedido</td><td>5</td></tr>
    <tr><td>02</td><td>US-02</td><td>Consultar historial de pedidos</td><td>3</td></tr>
    <tr><td>03</td><td>US-03</td><td>Editar pedidos</td><td>5</td></tr>
    <tr><td>04</td><td>US-04</td><td>Confirmar pedido recibido</td><td>3</td></tr>
    <tr><td>05</td><td>US-05</td><td>Actualización de un pedido</td><td>5</td></tr>
    <tr><td>06</td><td>US-06</td><td>Notificaciones a clientes sobre cambios</td><td>5</td></tr>
    <tr><td>07</td><td>US-07</td><td>Cancelación o rechazo de pedidos</td><td>3</td></tr>
    <tr><td>08</td><td>US-08</td><td>Inicio de sesión</td><td>3</td></tr>
    <tr><td>09</td><td>US-09</td><td>Registro de cuenta nueva</td><td>3</td></tr>
    <tr><td>10</td><td>US-10</td><td>Recuperación de contraseña</td><td>3</td></tr>
    <tr><td>11</td><td>US-11</td><td>Acceso restringido por roles</td><td>2</td></tr>
    <tr><td>12</td><td>US-12</td><td>Autenticación MFA para realizar pedidos</td><td>5</td></tr>
    <tr><td>13</td><td>US-13</td><td>Visualización del landing page</td><td>2</td></tr>
    <tr><td>14</td><td>TS-01</td><td>Implementar endpoint REST para pedidos</td><td>5</td></tr>
    <tr><td>15</td><td>TS-02</td><td>Servicio de autenticación y token</td><td>5</td></tr>
    <tr><td>16</td><td>TS-03</td><td>Envío de notificaciones por cambios de estado</td><td>3</td></tr>
    <tr><td>17</td><td>TS-04</td><td>Registro y validación de ubicación GPS</td><td>5</td></tr>
  </tbody>
</table>
