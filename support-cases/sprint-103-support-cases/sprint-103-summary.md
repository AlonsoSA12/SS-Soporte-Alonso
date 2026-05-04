# Soporte y mantenimiento - Sprint 103

Periodo base documentado: 20 de abril al 04 de mayo de 2026

## Resumen

Total de casos documentados: 26

Total de horas invertidas: 31.0 h

Este reporte consolida los casos de soporte y mantenimiento identificados para Singular Stories durante el Sprint 103. La documentacion se organiza por casos operativos, no por canales de Slack, siguiendo la estructura usada en reportes anteriores.

Nota: Los casos originados por conversaciones directas se documentan como soporte operativo, pero sus horas hombre se consolidan en un solo bloque para no fragmentar la estimacion por cada DM.

## Totales y segregacion de horas

### Segregacion por origen

| Origen | Casos incluidos | Horas |
|---|---:|---:|
| Casos de soporte con horas individuales | 13 casos | 19.5 h |
| Bloque de soporte por DMs | 13 casos | 11.5 h |
| **Total Sprint 103** | **26 casos** | **31.0 h** |

### Detalle de casos con horas individuales

| Caso | Horas |
|---|---:|
| Caso 1 - Error al crear historias por falta de creditos | 1.0 h |
| Caso 2 - Notificaciones de autorizacion no llegaban al PM correcto | 1.5 h |
| Caso 4 - Inconsistencia de OKRs entre Airtable y Singular Stories | 1.0 h |
| Caso 5 - No cargaban key projects al crear stories | 1.0 h |
| Caso 6 - Falla general al crear stories y tareas | 2.0 h |
| Caso 7 - Incidente S1 por imposibilidad de subir historias | 2.0 h |
| Caso 11 - Visualizacion incorrecta en Sprint Invoice | 1.5 h |
| Caso 12 - Overlap de componentes en laptops pequenas | 0.5 h |
| Caso 13 - Problemas al subir archivos en Talent Proof | 2.0 h |
| Caso 14 - View Story redirigia mal y Objectives generaban confusion | 2.0 h |
| Caso 17 - Oportunidades de mejora UX en Singular Stories | 0.75 h |
| Caso 18 - Correos de autenticacion de TW no llegaban | 1.25 h |
| Caso 19 - Rediseño de plataforma de subida de historias | 3.0 h |
| **Subtotal casos con horas individuales** | **19.5 h** |

### Detalle del bloque de DMs

| Bloque | Casos incluidos | Horas hombre |
|---|---:|---:|
| Soporte por DMs | 13 casos | 11.5 h |

Los casos incluidos en este bloque son: Caso 3, Caso 8, Caso 9, Caso 10, Caso 15, Caso 16, Caso DM-Miguel-01, Caso DM-Miguel-02, Caso DM-Miguel-03, Caso DM-Miguel-04, Caso DM-Miguel-05, Caso DM-Miguel-06 y Caso DM-Miguel-07.

### Segregacion por estado

| Estado | Casos | Horas |
|---|---:|---:|
| Resueltos o atendidos | 23 casos | 28.75 h |
| Pendientes o sin cierre visible | 3 casos | 2.25 h |
| **Total Sprint 103** | **26 casos** | **31.0 h** |

## Caso 1 - Error al crear historias por falta de creditos

Fecha: 20 de abril de 2026

### Contexto

Se reporto que al intentar crear historias en Singular Stories el flujo fallaba y no permitia avanzar. Inicialmente se sospecho una caida de n8n, porque el error afectaba directamente la generacion de stories.

### Acciones realizadas

Se reviso el flujo de creacion de historias, se valido el estado de las automatizaciones involucradas y se identifico que el bloqueo estaba relacionado con falta de creditos. Se coordino la compra temporal de creditos para restablecer el servicio y se notifico al equipo cuando el flujo volvio a estar operativo.

### Resultado

La creacion de historias quedo restablecida el mismo dia. El incidente se resolvio como una dependencia operativa de creditos y no como una falla funcional permanente de Singular Stories.

Horas invertidas: 1.0 h

## Caso 2 - Notificaciones de autorizacion no llegaban al PM correcto

Fecha: 21 al 22 de abril de 2026

### Contexto

Se reporto que cuando un developer enviaba una story para P4Auth, la notificacion no llegaba al PM correspondiente. En la revision del caso se detecto que, para el caso probado, la solicitud ni siquiera estaba llegando al servidor.

### Acciones realizadas

Se reviso el flujo de autorizacion, el caso reportado en Bloomer Health, la story SP-3 y la asignacion del talento involucrado. Se valido el comportamiento con el usuario que reporto el problema y se dio seguimiento hasta confirmar la recepcion correcta.

### Resultado

El flujo de notificacion quedo corregido y fue confirmado como resuelto por el usuario el 22 de abril.

Horas invertidas: 1.5 h

## Caso 3 - Revision de agente de Sprint Finish y TLDR

Fecha: 21 de abril de 2026

### Contexto

Se reporto que el agente de Sprint Finish seguia viendose incorrecto y que no estaba generando el TLDR esperado. El caso se reviso en una llamada rapida para validar si era un error del agente o una condicion del sprint.

### Acciones realizadas

Se reviso el sprint J2Academy Sprint 2 y se identifico que las tareas estaban en pending auth. Se explico que ese estado impedia generar correctamente el TLDR de Sprint Finish porque el sprint no tenia suficiente informacion autorizada para consolidar el cierre.

### Resultado

El comportamiento fue aclarado como una condicion de datos y estado del sprint, no como un bug directo del agente. El equipo quedo con contexto para continuar la revision de autorizaciones.

## Caso 4 - Inconsistencia de OKRs entre Airtable y Singular Stories

Fecha: 22 al 24 de abril de 2026

### Contexto

Se reporto que los valores mostrados en la seccion de OKRs no coincidian con Airtable. En particular, Singular Stories mostraba 4 KR cuando el objetivo tenia solo 3.

### Acciones realizadas

Se reviso la informacion mostrada en Singular Stories contra la fuente de datos en Airtable. Se dio seguimiento al reporte durante varios dias y se identifico que habia una dependencia con n8n que impedia avanzar completamente en la correccion durante el periodo revisado.

### Resultado

El caso quedo documentado como inconsistencia de datos con dependencia tecnica pendiente. No se encontro cierre visible dentro del periodo documentado.

Horas invertidas: 1.0 h

## Caso 5 - No cargaban key projects al crear stories

Fecha: 24 de abril de 2026

### Contexto

Se reporto que al crear stories no cargaban los key projects, lo que impedia continuar con el flujo de creacion.

### Acciones realizadas

Se reviso el flujo de creacion de stories y la carga de informacion necesaria para seleccionar key projects. Se aplico correccion sobre el bug y se pidio validacion al usuario que reporto el problema.

### Resultado

El flujo volvio a funcionar y el usuario confirmo que ya podia continuar con la creacion de stories.

Horas invertidas: 1.0 h

## Caso 6 - Falla general al crear stories y tareas

Fecha: 24 al 27 de abril de 2026

### Contexto

Varios usuarios reportaron fallos al crear stories y tareas. No aparecian campos como asignacion de talento, front/backend y tech stack. Tambien se reporto que la plataforma quedaba cargando epics, que no permitia sugerir nuevas epics y que habia fallos intermitentes de carga.

### Acciones realizadas

Se revisaron los reportes acumulados en soporte y bugs, se valido que el problema era general y se dio seguimiento con los usuarios afectados. Tambien se considero el impacto en celular, donde no se conservaban cookies, y se coordino la correccion del flujo para restablecer la creacion de stories.

### Resultado

El incidente fue escalado y posteriormente resuelto. La plataforma recupero la capacidad de crear stories y tareas con los campos requeridos.

Horas invertidas: 2.0 h

## Caso 7 - Incidente S1 por imposibilidad de subir historias

Fecha: 27 de abril de 2026

### Contexto

El problema de creacion de historias escalo a S1 porque varios talentos no podian crear stories. El sistema quedaba cargando key projects o no mostraba tech stack, afectando el avance operativo del sprint.

### Acciones realizadas

Se priorizo el incidente como critico, se revisaron los bloqueos principales del flujo y se propuso un workaround temporal en Airtable si el equipo necesitaba avanzar antes de la correccion definitiva. Se actualizo la plataforma y se pidio confirmacion a los usuarios afectados.

### Resultado

El incidente quedo resuelto el mismo 27 de abril. Se confirmo que la creacion de stories volvio a funcionar correctamente.

Horas invertidas: 2.0 h

## Caso 8 - Problema al proyectar recurso en Powderhouse

Fecha: 24 de abril de 2026

### Contexto

Se reporto que no era posible proyectar a Luis Esteban en el proyecto Powderhouse, aunque su utilizacion aparecia baja para las fechas requeridas.

### Acciones realizadas

Se reviso la informacion de utilizacion y se identifico que el problema estaba relacionado con datos de RRHH, especificamente con valores cargados en campos de horas diarias. Se coordino con Maria Eugenia la revision y ajuste de la informacion.

### Resultado

El dato fue corregido y el caso quedo resuelto. La proyeccion del recurso dejo de estar bloqueada por informacion incorrecta de capacidad.

## Caso 9 - Ajustes de roles de clientes y PM en Singular Stories

Fecha: 24 al 25 de abril de 2026

### Contexto

Se solicitaron ajustes de roles en Singular Stories para usuarios asociados a Osmomoney y para un talento que debia operar como Project Manager. Tambien se reviso la capacidad de impersonar usuarios desde el rol correspondiente.

### Acciones realizadas

Se asigno rol de cliente a los correos solicitados. Luego se reviso el rol requerido para Project Manager y se aclaro que los PM debian quedar como admins porque tambien necesitan impersonar. Se actualizo el rol del usuario solicitado y se valido que Maria Eugenia pudiera impersonar nuevamente.

### Resultado

Los usuarios quedaron configurados con los roles requeridos. La capacidad de impersonar quedo restablecida para el flujo operativo.

## Caso 10 - Revision de Utilization Budget para evaluaciones TW

Fecha: 24 al 25 de abril de 2026

### Contexto

Se necesitaba revisar informacion de Utilization Budget para permitir la generacion de evaluaciones de TW. La informacion debia estar lista para que el proceso de evaluaciones pudiera avanzar sin bloqueos de datos.

### Acciones realizadas

Se reviso la informacion asociada a Utilization Budget y se confirmo el estado al dia siguiente. Tambien se dio seguimiento con el equipo para validar que el dato quedara listo para el proceso de evaluaciones.

### Resultado

La informacion quedo preparada para continuar con la generacion de evaluaciones de TW.

## Caso 11 - Visualizacion incorrecta en Sprint Invoice

Fecha: 28 de abril de 2026

### Contexto

Se reporto que en Sprint Invoice el cliente veia un monto que no coincidia con lo facturado. Esto generaba confusion comercial y podia afectar la confianza del cliente en la informacion mostrada.

### Acciones realizadas

Se reviso la pantalla de Sprint Invoice y se comparo la informacion mostrada contra los campos correctos de facturacion. Se identifico que la vista estaba mostrando un campo incorrecto o ambiguo y se ajusto la informacion visible para el cliente.

### Resultado

La pantalla quedo actualizada para mostrar el campo correcto del Sprint Invoice. El caso se resolvio como mantenimiento correctivo funcional.

Horas invertidas: 1.5 h

## Caso 12 - Overlap de componentes en laptops pequenas

Fecha: 28 de abril de 2026

### Contexto

Se reporto que en pantallas de laptop menores a 15 pulgadas habia overlap de componentes en Singular Stories.

### Acciones realizadas

Se documento el problema de visualizacion y se clasifico como mantenimiento correctivo de UX. El caso quedo identificado para revision de layout responsivo.

### Resultado

No se encontro cierre visible dentro del periodo documentado. Queda como pendiente de ajuste visual.

Horas invertidas: 0.5 h

## Caso 13 - Problemas al subir archivos en Talent Proof

Fecha: 28 de abril de 2026

### Contexto

Se reporto que al subir 3 archivos en Talent Proof, en algunos casos desaparecia 1 o 2 archivos. Esto afectaba la confiabilidad del flujo de carga de evidencias.

### Acciones realizadas

Se reviso el comportamiento de carga de archivos y se identifico que el problema estaba relacionado con la configuracion de buckets en Vercel para la plataforma de subir historias de usuario. Se realizaron los cambios necesarios en la configuracion, se valido nuevamente el flujo de subida y se hizo deploy de la plataforma para publicar la correccion.

### Resultado

El caso quedo resuelto. La carga de archivos en Talent Proof volvio a funcionar correctamente despues de corregir la configuracion de buckets en Vercel y redeployar la plataforma.

Horas invertidas: 2.0 h

## Caso 14 - View Story redirigia mal y los Objectives generaban confusion

Fecha: 28 al 29 de abril de 2026

### Contexto

Se reporto que el boton View Story enviaba al dashboard en lugar de abrir la historia. Esto hacia que clientes no pudieran revisar historias y pudieran aprobarlas sin ver el detalle. Tambien se reporto confusion por la forma en que se mostraban los Objectives.

### Acciones realizadas

Se investigo el cambio de rutas generado despues de deshabilitar el formulario manual anterior. Se actualizaron los campos Link Story Noloco, URL Singular Stories y URL Singular Stories Talent Proof. Tambien se ajusto la visualizacion de Objectives para reducir la confusion del cliente, quitando el codigo del Objective y aplicando el ajuste en las pantallas correspondientes.

### Resultado

View Story quedo direccionando correctamente y los Objectives fueron ajustados visualmente sin el codigo que generaba ruido en la lectura. El incidente se resolvio como mantenimiento correctivo critico por impacto en aprobacion de historias.

Horas invertidas: 2.0 h

## Caso 15 - Desactivacion de automatizaciones Slack y aprobaciones automaticas

Fecha: 29 de abril de 2026

### Contexto

Se solicito desactivar automatizaciones diarias de Slack en canales internos y revisar un mensaje automatico de aprobacion de historias que se enviaba sin que Miguel o Laura presionaran el boton correspondiente.

### Acciones realizadas

Se desactivaron las automatizaciones de Slack solicitadas. Luego se reviso el flujo de Pipedream asociado a aprobaciones de Singular Stories y se identifico que el mensaje estaba programado para enviarse de lunes a viernes. Se retiro la ejecucion automatica para que el envio quedara condicionado a la accion manual.

### Resultado

Las automatizaciones quedaron ajustadas. Los recordatorios y aprobaciones dejaron de ejecutarse automaticamente fuera del flujo esperado.

## Caso 16 - Seguimiento de Cohorts y resultados TW

Fecha: 29 de abril de 2026

### Contexto

Se consulto por los Cohorts de TW porque solo se veian resultados de 15 personas sobre un universo mayor de colaboradores. Era necesario aclarar si el resultado era incompleto o si respondia a criterios de elegibilidad.

### Acciones realizadas

Se reviso la informacion de resultados generados y se aclaro que solo 15 personas calificaban para el resultado, aunque habia 39 personas involucradas entre evaluados y evaluadores. Tambien se confirmo que los resultados podian regenerarse despues de completar evaluaciones pendientes.

### Resultado

El equipo quedo con claridad sobre el alcance de los resultados visibles y la posibilidad de regenerar Cohorts luego de completar pendientes.

## Caso DM-Miguel-01 - Seguimiento de creditos OpenAI para generacion de stories

Fecha: 21 de abril de 2026

### Contexto

Miguel consulto por cargos adicionales de OpenAI asociados a creditos y configuracion de API. El punto era relevante para Singular Stories porque la generacion de stories depende de consumo de API y necesitaba quedar operativa sin bloquear la creacion de historias.

### Acciones realizadas

Se explico que los cargos correspondian a recargas de creditos y a la activacion de auto recarga en las cuentas usadas para API. Se dio contexto del consumo y se mantuvo seguimiento para evitar nuevos bloqueos por falta de creditos.

### Resultado

Miguel quedo con la informacion necesaria para justificar los cargos y el flujo de generacion de stories mantuvo continuidad operativa.

## Caso DM-Miguel-02 - Rotacion de secrets para app de story generation

Fecha: 22 de abril de 2026

### Contexto

Miguel compartio el pedido de rotar secrets para la app de story generation desarrollada para Singular Stories. El objetivo era reducir riesgo operativo y mantener la configuracion segura despues de la solicitud del equipo.

### Acciones realizadas

Se tomo el requerimiento, se priorizo junto con la planificacion activa del sprint y se preparo el cambio de secrets requerido para la app de generacion de stories.

### Resultado

El caso quedo atendido como mantenimiento preventivo de seguridad para el flujo de story generation.

## Caso DM-Miguel-03 - Seguimiento de Trustworthiness bot antes de evaluaciones

Fecha: 23 de abril de 2026

### Contexto

Se dio seguimiento con Miguel al estado del bot de Trustworthiness antes del inicio de evaluaciones. La prioridad era mantener el flujo actual operativo, evitar cambios de logica antes de validarlo con uso real y mejorar la calidad de respuestas.

### Acciones realizadas

Se compartio el plan de trabajo sobre el bot, incluyendo mantener el flujo base, evaluar DeepSeek como agente guia, revisar tiempos de respuesta y simplificar la interfaz porque estaba muy cargada. Tambien se explico la condicion de consumo de DeepSeek y la necesidad de registrar tarjeta para probar performance real.

### Resultado

Miguel recibio contexto del estado tecnico y de producto del bot. El trabajo quedo enfocado en iterar sobre feedback real, mejorar UI y validar performance sin rehacer el flujo antes de las evaluaciones.

## Caso DM-Miguel-04 - Renovacion de Pipedream para ejecucion de TW

Fecha: 27 de abril de 2026

### Contexto

Se detecto que los nuevos procesos de TW no se ejecutaron porque la plataforma de Pipedream no se habia renovado. Esto afectaba automatizaciones usadas para Trustworthiness y podia impactar la generacion de evaluaciones.

### Acciones realizadas

Se notifico a Miguel la causa del problema, se coordino el uso de su tarjeta para renovar Pipedream y se priorizo la reactivacion por impacto en los TW.

### Resultado

El origen del bloqueo quedo identificado y se gestiono la renovacion para restablecer la ejecucion de automatizaciones relacionadas con TW.

## Caso DM-Miguel-05 - Revision de migracion de base de datos de Singular Stories

Fecha: 30 de abril de 2026

### Contexto

Se solicito una llamada con Miguel para revisar un punto relacionado con la migracion de base de datos de Singular Stories. El objetivo era no perder el contexto tecnico antes de continuar con los cambios del sprint.

### Acciones realizadas

Se realizo una llamada breve para revisar el tema de migracion de base de datos y alinear el siguiente paso tecnico.

### Resultado

El punto quedo revisado con Miguel y se mantuvo continuidad sobre el analisis de base de datos de Singular Stories.

## Caso DM-Miguel-06 - Continuidad de Google Cloud, Firebase y n8n de Singular Stories

Fecha: 01 de mayo de 2026

### Contexto

Se detecto riesgo de caida en Google Cloud por falta de pago. La cuenta involucrada correspondia al entorno administrador de Singular en Firebase, donde viven automatizaciones de cohorts, Singular Stories, carga de data para creacion de historias, carga de data de QA y n8n.

### Acciones realizadas

Se solicito la tarjeta a Miguel, se explico el alcance del entorno afectado y se registro el concepto del cargo como Google Cloud Platform para el proyecto Singular Stories FF. Tambien se aclaro que el entorno incluia n8n de Singular.

### Resultado

El pago quedo realizado y se evito la caida del entorno de Google Cloud/Firebase usado por Singular Stories y automatizaciones relacionadas.

## Caso DM-Miguel-07 - Renovacion de Pipedream para aprobaciones de Singular Stories

Fecha: 04 de mayo de 2026

### Contexto

Se necesito completar una verificacion y pago relacionado con Pipedream. La automatizacion afectada se usa para que talentos soliciten aprobacion de PO y PM, y tambien para que clientes aprueben tareas por Slack.

### Acciones realizadas

Se coordino con Miguel la verificacion por codigo, se completo el pago de Pipedream y se explico el concepto del cargo para su registro.

### Resultado

Pipedream quedo renovado y las automatizaciones de aprobacion de Singular Stories mantuvieron continuidad operativa.

## Horas hombre - Bloque de soporte por DMs

Casos incluidos: Caso 3, Caso 8, Caso 9, Caso 10, Caso 15, Caso 16, Caso DM-Miguel-01, Caso DM-Miguel-02, Caso DM-Miguel-03, Caso DM-Miguel-04, Caso DM-Miguel-05, Caso DM-Miguel-06 y Caso DM-Miguel-07.

Horas hombre invertidas: 11.5 h

## Caso 17 - Oportunidades de mejora UX en Singular Stories

Fecha: 28 de abril de 2026

### Contexto

Se identificaron oportunidades de mejora en la experiencia de Singular Stories, incluyendo scroll horizontal poco intuitivo en stories, necesidad de visualizar tareas desglosadas por sprint para clientes FTE/HTE y mayor prioridad visual para OKRs en el dashboard.

### Acciones realizadas

Se documentaron los puntos de mejora y se pidio una llamada para aterrizar mejor el alcance. Los puntos fueron clasificados como mantenimiento evolutivo y mejora continua, no como bugs bloqueantes inmediatos.

### Resultado

Las mejoras quedaron abiertas para definicion de alcance y priorizacion posterior.

Horas invertidas: 0.75 h

## Caso 18 - Correos de autenticacion de TW no llegaban

Fecha: 04 de mayo de 2026

### Contexto

Se reporto que no llegaba el correo de autenticacion para realizar evaluaciones de TW, incluso despues de probar varias veces, en diferentes navegadores y luego de borrar cache.

### Acciones realizadas

Se reviso el flujo de autenticacion y las automatizaciones asociadas. Se identifico que una automatizacion de Make estaba apagada. Se reactivo el proceso y se hicieron pruebas con codigos nuevos hasta confirmar la recepcion del correo.

### Resultado

El problema quedo resuelto el mismo 04 de mayo. El usuario confirmo que el correo ya llegaba correctamente.

Horas invertidas: 1.25 h

## Caso 19 - Rediseño de plataforma de subida de historias

Fecha: Sprint 103

### Contexto

La plataforma de subir historias de usuario necesitaba alinearse visualmente con el design system definido por Cesar para el proyecto de Singular Stories. El objetivo era mejorar la consistencia visual, la claridad del flujo y la percepcion de calidad de la herramienta usada para cargar historias.

### Acciones realizadas

Se mejoro el diseño completo de la plataforma de subida de historias, ajustando la interfaz al design system definido para Singular Stories. Se revisaron estilos, estructura visual, jerarquia de informacion y componentes principales para que la experiencia quedara alineada con el resto del producto.

### Resultado

La plataforma quedo visualmente actualizada y alineada al design system de Singular Stories. El cambio mejora la coherencia del producto y reduce la friccion visual en el flujo de carga de historias de usuario.

Horas invertidas: 3.0 h

## Comentarios de cierre

El Sprint 103 concentro la mayor parte del soporte en Singular Stories, especialmente en creacion de historias, aprobaciones, rutas de visualizacion, automatizaciones, datos requeridos para TW y mejoras de consistencia visual en la plataforma de carga de historias. El incidente de mayor impacto fue la imposibilidad de crear historias, clasificado como S1 y resuelto durante el sprint.

Quedan documentados como pendientes o sin cierre visible la inconsistencia de OKRs, el overlap en laptops pequenas y las mejoras UX abiertas para priorizacion posterior.
