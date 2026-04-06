# Soporte y mantenimiento - Sprint 100

Periodo base documentado: 17 de marzo al 19 de marzo de 2026

## Caso 1 - Correccion de automatizacion de aprobacion de historias en Slack

**Fecha:** 17 de marzo de 2026

### Contexto
Se reviso en Pipedream por que no estaba llegando el mensaje de aprobacion de historias en Slack. Durante la revision se identificaron errores por tipos de datos y caracteres especiales dentro de la automatizacion. Tambien se confirmo que, en algunas pruebas, no se enviaba mensaje porque no habia historias en estado pendiente de aprobacion del cliente.

### Acciones realizadas
- Se reviso la automatizacion en Pipedream.
- Se busco el error dentro del flujo.
- Se identificaron errores por tipos de datos y caracteres especiales.
- Se aplicaron correcciones.
- Se compartieron accesos de Pipedream con Camila para que tambien pudiera ingresar a revisar el flujo.
- Se realizaron pruebas en test.
- Se desplego la correccion.
- Se pauso el mensaje de "no hay stories".
- Se espero a que actualizaran el estado para volver a ejecutar la automatizacion.

### Resultado
La automatizacion quedo corregida a nivel tecnico en Pipedream y se confirmo que el mensaje normal de aprobacion dependia de que existieran historias en el estado correspondiente. Camila tambien quedo con acceso al flujo para futuras revisiones.

**SPs:** 4
**Horas invertidas:** 4.0 h

## Caso 2 - Eliminacion de mensajes enviados por error en Slack

**Fecha:** 17 de marzo de 2026

### Contexto
Se enviaron por error mensajes en Slack indicando que no habia historias pendientes de aprobacion del cliente. Fue necesario pedir apoyo para eliminarlos y evitar confusion en el canal correspondiente.

### Acciones realizadas
- Se identificaron los mensajes enviados por error.
- Se compartieron los enlaces de los mensajes a Maria Eugenia.
- Se solicito la eliminacion de los mensajes en Slack.
- Se confirmo la eliminacion de los mensajes.

### Resultado
Los mensajes enviados por error fueron eliminados de Slack y se evito que continuaran visibles en el canal.

**Horas invertidas:** 0.5 h

## Caso 3 - Ajuste de roles de usuario y accesos QA

**Fecha:** 19 de marzo de 2026

### Contexto
Maria Eugenia solicito corregir el rol de un cliente que aparecia como recurso en lugar de cliente y tambien habilitar la configuracion de usuario QA para dos personas a las que no les aparecia la seccion de QA Path.

### Acciones realizadas
- Se reviso el usuario con correo `stef@stefbloom.com`.
- Se actualizo su rol para que quedara como cliente.
- Se registro el nombre `Stef` para el usuario en Singular.
- Se reviso el acceso QA para `operdomo@singularagency.co`.
- Se habilito la configuracion de usuario QA para `operdomo@singularagency.co`.
- Se habilito la configuracion de usuario QA para `zmejia@singularagency.co`.

### Resultado
El usuario `stef@stefbloom.com` quedo con rol de cliente y los usuarios `operdomo@singularagency.co` y `zmejia@singularagency.co` quedaron con configuracion de QA habilitada para su acceso correspondiente.

**Horas invertidas:** 0.5 h

## Caso 4 - Creacion de TW Cohorts History y ajuste de registros sin resource

**Fecha:** 19 de marzo de 2026

### Contexto
Will consulto si el historico de TW habia quedado automatizado y reporto que el registro de Juan Berti solo llegaba hasta enero, por lo que parecia faltar la informacion de febrero. Tambien se empezo la automatizacion de `TW Cohorts History`, pero el trabajo quedo a la mitad porque Airtable estaba caido el viernes y no permitia seleccionar campos para conectar `Cohorts` con la tabla `Cohorts History`.

### Acciones realizadas
- Se confirmo que el historico no habia quedado automatico, pero estaba actualizado.
- Se empezo la automatizacion de `TW Cohorts History`.
- Despues de lanzar los cohorts de los talentos, se avanzo en la conexion con la tabla `TW Cohorts History`.
- Se reviso la automatizacion creada para el historico de TW.
- Se identifico que Airtable no permitia seleccionar campos para conectar `Cohorts` con la tabla `Cohorts History`.
- Se identifico una dificultad al editar el campo `resource`, ya que el navegador se colgaba al intentar seleccionarlo.
- Se valido si el problema correspondia a una fecha o a otra condicion en los registros.
- Se detectaron 5 records con el campo `resource` vacio.
- Se actualizaron los records que tenian el campo `resource` vacio.

### Resultado
Se confirmo que el problema no era de fechas. La automatizacion de `TW Cohorts History` avanzo hasta la mitad, pero no pudo completarse por la caida de Airtable al momento de seleccionar campos para la conexion entre tablas. Los registros con `resource` vacio fueron actualizados, dejando el historico de TW al dia en esa parte del proceso.

**Horas invertidas:** 1.5 h

## Caso 5 - Revision de visibilidad de opcion non billable para cliente

**Fecha:** 19 de marzo de 2026

### Contexto
Laura reporto que un cliente todavia podia ver la opcion para marcar tareas como `non billable` en la vista de `active-sprint`. Indico que recordaba una solicitud previa para que ese tipo de informacion no estuviera visible para clientes.

### Acciones realizadas
- Se solicito la URL donde se visualizaba el campo.
- Se reviso la ruta `https://www.singular-stories.com/active-sprint`.
- Se consulto con que cuenta estaba viendo Laura el comportamiento reportado.
- Se confirmo el correo del cliente `cmonge@outlook.com`.
- Se reviso si la solicitud previa correspondia al card de `pre work` que mostraba el total de `non billable`, el cual ya habia sido retirado.
- Se planteo la necesidad de confirmar el requerimiento, ya que ocultar el campo tambien impediria al cliente ver si una tarea era billable o no.

### Resultado
El caso quedo en revision funcional y pendiente de confirmacion con Juanse para definir si la opcion `non billable` debe ocultarse para clientes en esa vista.

**Horas invertidas:** 0.5 h
