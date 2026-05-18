# Informe de soporte y menimiento 104

## Resumen Ejecutivo

Se identificaron 31 casos relevantes de soporte o mantenimiento dentro del alcance revisado.

- Total de casos de soporte: 17.
- Total de casos de mantenimiento: 14.
- Sistemas mas afectados: Singular Stories, SS Client, Airtable/Operaciones, Pipedream/N8N/PostHog, Google Calendar/Make.
- Personas que mas solicitaron soporte o mantenimiento: Laura Aguirre, Miguel Perez, Gerardo Molina, Silvia M. Dubon, Camila Andrea Ruge, Esteban Mena, Claudia Galdamez.
- Riesgos principales: metadata historica de aprobaciones no recuperable completamente, dependencia de logs con retencion limitada, tareas movidas de sprint sin cierre visible, automatizaciones duplicadas, dependencias de permisos/admin externos y soporte operativo no planificado.

Estados usados:

- Resuelto: hay confirmacion explicita, validacion posterior, agradecimiento o evidencia de cierre.
- Pendiente: hay solicitud de accion sin cierre visible.
- Bloqueado: se menciona acceso, permiso, dato o dependencia externa faltante.
- Sin evidencia suficiente: la conversacion queda parcial o no permite confirmar estado.

## Timeline Por Dia

### 2026-05-05

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| #ss-internal-team | Updates de diagramas: modo light/night, titulo, leyenda, descarga y pruebas con Esteban. | Alonso / feedback de equipo | Mantenimiento | Resuelto parcialmente; hubo feedback posterior sobre render/flujo. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1777989724917579) |
| Grupo Alonso, Maria Eugenia, Silvia | Cambiar a Amy de MAC7 a cliente y compartir magic link. | Silvia M. Dubon | Mantenimiento | Resuelto; Alonso cambio el recurso a client y compartio link de invitacion; Silvia agradece. | [Slack](https://singular-innovation.slack.com/archives/C09AUS5TYFP/p1778007034910169) |

### 2026-05-06

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| DM Andres Rebuly | Singular Agile no permitia cambiar status de stories. | Andres Rebuly Pineda | Mantenimiento | Resuelto; Alonso dio permisos y Andres confirmo que ya le dejaba. | [Slack](https://singular-innovation.slack.com/archives/D0B1ZQ3ATAS/p1778097521775679) |
| DM Maria Eugenia | Generacion de cohorts; ejecucion se quedo trabada a media ruta. | Maria Eugenia Garcia | Soporte | Resuelto; Alonso luego confirma que cohorts ya quedo. | [Slack](https://singular-innovation.slack.com/archives/D09AUS5HXPF/p1778079286891889) |
| DM Miguel | Explicar donde se guardan/consultan diagramas creados por talentos, POs y PMs. | Miguel Perez | Mantenimiento | Resuelto con video posterior en canal interno. | [Slack](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778108592909989) |

### 2026-05-07

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| #ss-internal-team | Implementar diagramas para historias antiguas. | Miguel Perez / Laura Aguirre | Mantenimiento | Resuelto; Alonso comparte video tutorial y Miguel valida. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778165168703329) |
| #ss-internal-team | Agregar Respon.io como stack. | Laura Aguirre | Mantenimiento | Resuelto; Alonso responde "Voy" y luego "listo". | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778190259709569) |
| #review-invoice | Corregir MLE historico e invoice_for_clients_ss para Powderhouse y luego otros proyectos. | Miguel Perez / Laura Aguirre | Soporte | Parcialmente resuelto para Powderhouse; expansion a otros proyectos quedo como trabajo posterior. | [Slack](https://singular-innovation.slack.com/archives/C0B27D9HXHR/p1778196819621129) |
| #soporte_singular-stories | Llamada urgente por soporte de SS. | Gerardo Molina | Soporte | Derivo en investigacion de invoice/metadata y aprobaciones; cierre final no queda en ese canal. | [Slack](https://singular-innovation.slack.com/archives/C03LWCRFCJF/p1778192436988309) |

### 2026-05-08

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| DM Miguel | Alejandra no podia impersonar otro usuario. | Miguel Perez | Soporte | Resuelto para proyecto/correo correcto; Alonso confirma proyecto de Hera en Estimation. | [Slack](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778254240690589) |
| #review-invoice | Issue de metadata en aprobaciones. | Miguel Perez | Soporte | Investigacion abierta; Alonso indica que Pipedream/N8N guardan por tiempo limitado. | [Slack](https://singular-innovation.slack.com/archives/C0B27D9HXHR/p1778251492501619) |
| DM Miguel | Error de aprobacion masiva: Sprint View no enviaba email y quedaba unknown. | Alonso / Miguel | Soporte | Fix implementado para que deje de ocurrir; historico unknown no recuperable totalmente. | [Slack](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778265701000000) |
| DM Luis / DM Claudia / DM Camila | Buscar logs en N8N, Pipedream y PostHog para recuperar trazabilidad. | Alonso / Miguel | Mantenimiento | Bloqueado/parcial; N8N community borra historial a diario y Pipedream/PostHog tienen retencion limitada. | [Slack](https://singular-innovation.slack.com/archives/D0933ANGN86/p1778257078000000) |
| Grupo Gerardo, Alonso, Jorge, Miguel | Reporte de ultimos 3 sprints con aprobaciones; facturas frenadas. | Gerardo Molina | Soporte | Parcialmente resuelto; Alonso preparo reporte/video, pero indica que algunos unknown no tienen fuente recuperable. | [Slack](https://singular-innovation.slack.com/archives/C0B2F6NPKEX/p1778265071000000) |

### 2026-05-11

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| DM Miguel | Explicar y documentar fix de approvals unknown. | Miguel Perez | Soporte | Resuelto; Alonso describe causa y fix: agregar email al request del Sprint View. | [Slack](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778506788000000) |
| Grupo Alejandra, Alonso, Miguel, Marlin, Laura, Camila | Talento aparecia como no pagado aunque el sprint estaba pagado. | Alejandra Ramirez | Soporte | Resuelto por Camila; causa raiz: espacio final en Referencia a Proyecto que rompia filtro. | [Slack](https://singular-innovation.slack.com/archives/C0B3NK0HBL2/p1778529886000000) |
| DM Laura | Talentos no podian pasar tareas a in progress o quedaba lento. | Laura Aguirre | Soporte | Sin evidencia suficiente; Alonso prueba y sugiere refresh/limpiar memoria, posible Noco/NoLoco. | [Slack](https://singular-innovation.slack.com/archives/D096KML3TRV/p1778533146000000) |

### 2026-05-12

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| Grupo Alonso, Miguel, Camila, Guillermo | A Guillermo no le aparecian stories de Housing Research. | Miguel Perez | Soporte | Resuelto; Camila confirma "Ya quedo resuelto" y Miguel agradece. | [Slack](https://singular-innovation.slack.com/archives/C0B2W0S3RPH/p1778601988000000) |
| DM Maria Eugenia | Documentacion TW / RRHH. | Maria Eugenia Garcia | Mantenimiento | Resuelto; Alonso comparte documento de informe RRHH_calculo actual del TW. | [Slack](https://singular-innovation.slack.com/archives/D09AUS5HXPF/p1778600000000000) |

### 2026-05-13

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| #singular-stories-2026 | URL de ultima version deployada de SS Client. | Cesar / Amilkar | Mantenimiento | Compartido y validado con reacciones; evidencia de deploy disponible. | [Slack](https://singular-innovation.slack.com/archives/C077DM3QSHG/p1778684170213489) |
| Grupo Alejandra, Alonso, Miguel, Marlin, Laura, Camila | Calculo de SPs trabajados no concordaba con valor por SP. | Marlin Lopez | Soporte | Resuelto; Marlin confirma que ya aparece modificado. | [Slack](https://singular-innovation.slack.com/archives/C0B3NK0HBL2/p1778701424000000) |

### 2026-05-14

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| #ss-internal-team / DM Laura | Automatizaciones de Slack duplicadas y remover automatizacion. | Laura Aguirre | Soporte | Resuelto inferido; Alonso responde "Voy" y Laura agradece. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778767513068749) |
| #ss-internal-team | Al subir SS aparece warning y no deja. | Esteban Mena | Soporte | Resuelto; se trabajo en Vercel y ya fue visto. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778768437741919) |
| DM Miguel | Riesgo de eliminar correos/automatizaciones de cb y mperera. | Miguel Perez | Mantenimiento | Pendiente/conservador; Alonso advierte que no hay certeza de que puede romper. | [Slack](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778772719000000) |

### 2026-05-15

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| DM Laura | Call Center: cliente no podia aprobar post QA approval en sprints 24/25. | Laura Aguirre | Soporte | Resuelto; Laura confirmo cierre despues de la validacion local de Alonso. | [Slack](https://singular-innovation.slack.com/archives/D096KML3TRV/p1778846087000000) |

### 2026-05-18

| Bloque | Solicitud o tema | Quien lo pidio | Tipo | Resultado visible | Evidencia |
|---|---|---:|---|---|---|
| DM Laura | Tarea de auditoria/facturas; decidir si se pasa al siguiente sprint. | Laura Aguirre | Mantenimiento | Pendiente/movida; se acuerda pasarla y dejarla done entre lunes y martes. | [Slack](https://singular-innovation.slack.com/archives/D096KML3TRV/p1779114005000000) |
| #ss-internal-team | Confirmar que hay de lo trabajado en prod. | Laura Aguirre | Mantenimiento | Pendiente; thread no expone cierre visible en lectura. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1779119320950329) |
| #ss-internal-team | Confirmar Supabase listo para conexion de SS Client al 22. | Miguel Perez | Mantenimiento | Pendiente; no hay cierre visible en lectura. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1779119483881939) |
| #ss-internal-team | Fix de texto que se sobrepone. | Esteban Mena | Soporte | Resuelto; se trabajo en Vercel y ya fue visto. | [Slack](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1779120735920519) |
| Grupo Claudia, Alonso, Miguel, Laura | Tarea en ideation no puede volver al wizard/AI story generator con campos prefilled. | Claudia Galdamez / Miguel Perez | Soporte | Pendiente/backlog; Alonso propone subirlo como KP para trabajarlo. | [Slack](https://singular-innovation.slack.com/archives/C0B4DKWCC7M/p1779127727000000) |
| DM Camila | Automatizacion de coaching con Google Calendar; permisos Make/noreply. | Camila Andrea Ruge | Mantenimiento | Bloqueado por permisos/conocimiento de cuenta; Alonso sugiere pedir permisos a Amilkar. | [Slack](https://singular-innovation.slack.com/archives/D0ACW67NWGM/p1779130000000000) |

## Matriz Consolidada

| Fecha | Hora | Bloque | Solicitante | Proyecto/Sistema | Descripcion exacta | Tipo | Urgencia aparente | Respuesta de Alonso | Estado inferido | Link Slack |
|---|---:|---|---|---|---|---|---|---|---|---|
| 2026-05-05 | 09:02 | #ss-internal-team | Equipo SS | Singular Stories | Updates de diagramas: light/night, titulo, leyenda, descarga. | Mantenimiento | Media | Comparte cambios y pide feedback/pruebas. | Resuelto parcial | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1777989724917579) |
| 2026-05-05 | 13:50 | Grupo Alonso/Maria/Silvia | Silvia M. Dubon | Singular Stories | Cambiar amy@mac7propertyservices.com a client y compartir magic link. | Mantenimiento | Alta | Cambia recurso a client y envia link. | Resuelto | [link](https://singular-innovation.slack.com/archives/C09AUS5TYFP/p1778007034910169) |
| 2026-05-06 | 11:58 | DM Andres | Andres Rebuly | Singular Agile | No permite cambiar status de stories. | Mantenimiento | Media | Da permisos. | Resuelto | [link](https://singular-innovation.slack.com/archives/D0B1ZQ3ATAS/p1778097521775679) |
| 2026-05-06 | 17:03 | DM Miguel | Miguel Perez | Singular Stories | Ayudar a Laura a entender donde se guardan diagramas. | Mantenimiento | Media | Coordina video y explicacion. | Resuelto | [link](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778108592909989) |
| 2026-05-07 | 09:46 | #ss-internal-team | Miguel/Laura | Singular Stories | Diagramas para historias antiguas. | Mantenimiento | Media | Comparte video tutorial. | Resuelto | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778165168703329) |
| 2026-05-07 | 16:44 | #ss-internal-team | Laura Aguirre | Singular Stories | Agregar Respon.io como stack. | Mantenimiento | Alta | "Voy" y luego "listo". | Resuelto | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778190259709569) |
| 2026-05-07 | 18:33 | #review-invoice | Miguel Perez | SS Invoice / Airtable | MLE historico e invoice_for_clients_ss para Powderhouse. | Soporte | Alta | Explica plan, crea campo historico y obtiene data. | Resuelto parcial | [link](https://singular-innovation.slack.com/archives/C0B27D9HXHR/p1778196819621129) |
| 2026-05-07 | 17:20 | #soporte_singular-stories | Gerardo Molina | Singular Stories | Llamada urgente de soporte. | Soporte | Critica | Toma caso y deriva actualizaciones a review-invoice/grupo. | Sin evidencia suficiente | [link](https://singular-innovation.slack.com/archives/C03LWCRFCJF/p1778192436988309) |
| 2026-05-08 | 10:30 | DM Miguel | Miguel Perez | Singular Stories | Alejandra no puede impersonar. | Soporte | Alta | Verifica correo/proyecto y confirma ajuste. | Resuelto | [link](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778254240690589) |
| 2026-05-08 | 09:44 | #review-invoice | Miguel Perez | SS approvals | Metadata de aprobaciones aparece incorrecta/unknown. | Soporte | Critica | Revisa Pipedream/N8N y datos. | Parcial | [link](https://singular-innovation.slack.com/archives/C0B27D9HXHR/p1778251492501619) |
| 2026-05-08 | 13:41 | DM Miguel | Alonso/Miguel | SS approvals | Sprint View no enviaba email en aprobacion masiva. | Soporte | Critica | Encuentra causa y plantea fix; luego lo documenta. | Resuelto hacia adelante | [link](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778265701000000) |
| 2026-05-08 | 11:17 | DM Luis | Alonso | N8N | Consultar historial de escenario antiguo. | Mantenimiento | Alta | Pregunta por logs; Luis indica borrado diario por default. | Bloqueado | [link](https://singular-innovation.slack.com/archives/D0933ANGN86/p1778257078000000) |
| 2026-05-08 | 14:01 | DM Claudia | Alonso | PostHog SS | Solicitar acceso a PostHog y recordings. | Mantenimiento | Alta | Pide acceso e invitar a Miguel. | Parcial | [link](https://singular-innovation.slack.com/archives/D043ZKLAWJW/p1778266905000000) |
| 2026-05-08 | 18:31 | Grupo Gerardo/Alonso/Jorge/Miguel | Gerardo Molina | SS approvals / invoices | Reporte de sprints con aprobaciones y facturas frenadas. | Soporte | Critica | Explica limites y luego comparte reporte/video. | Parcial | [link](https://singular-innovation.slack.com/archives/C0B2F6NPKEX/p1778283071000000) |
| 2026-05-11 | 09:39 | DM Miguel | Miguel Perez | SS approvals | Documentar fix para que no vuelva a guardarse unknown. | Soporte | Alta | Explica causa y fix con detalle. | Resuelto | [link](https://singular-innovation.slack.com/archives/D09K7SQJTBQ/p1778506788000000) |
| 2026-05-11 | 12:04 | Grupo Alejandra/Miguel/Laura/Camila | Alejandra Ramirez | SS pagos | Talento aparece no pagado aunque ya se pago. | Soporte | Alta | Alonso deriva a Camila por carga de soporte. | Resuelto | [link](https://singular-innovation.slack.com/archives/C0B3NK0HBL2/p1778519086000000) |
| 2026-05-11 | 14:52 | DM Laura | Laura Aguirre | SS/Noco | Error al pasar tareas a in progress o lentitud. | Soporte | Media | Prueba y sugiere refresh/limpiar memoria. | Sin evidencia suficiente | [link](https://singular-innovation.slack.com/archives/D096KML3TRV/p1778529155000000) |
| 2026-05-12 | 11:06 | Grupo Alonso/Miguel/Camila/Guillermo | Miguel Perez | SS Housing Research | Stories no visibles para Guillermo. | Soporte | Alta | Camila toma caso. | Resuelto | [link](https://singular-innovation.slack.com/archives/C0B2W0S3RPH/p1778598388000000) |
| 2026-05-13 | 09:56 | #singular-stories-2026 | Cesar/Amilkar | SS Client | Compartir URL deployada de ultima version. | Mantenimiento | Media | Canal valida con reacciones. | Resuelto | [link](https://singular-innovation.slack.com/archives/C077DM3QSHG/p1778684170213489) |
| 2026-05-13 | 14:43 | Grupo Alejandra/Miguel/Laura/Camila | Marlin Lopez | SS pagos/SP | Calculo de SPs trabajados no corresponde al valor por SP. | Soporte | Alta | Se revisa en llamada. | Resuelto | [link](https://singular-innovation.slack.com/archives/C0B3NK0HBL2/p1778701424000000) |
| 2026-05-14 | 09:05 | #ss-internal-team | Laura Aguirre | Slack automations | Automatizaciones enviandose dos veces. | Soporte | Alta | Alonso atiende por DM y dice "Voy". | Resuelto inferido | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778767513068749) |
| 2026-05-14 | 09:20 | #ss-internal-team | Esteban Mena | Singular Stories | Warning al subir SS y no deja. | Soporte | Media | Se trabajo en Vercel y ya fue visto. | Resuelto | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1778768437741919) |
| 2026-05-15 | 08:54 | DM Laura | Laura Aguirre | SS Call Center | Cliente no puede aprobar post QA approval. | Soporte | Critica | Alonso valida localmente; Laura confirmo que cerro. | Resuelto | [link](https://singular-innovation.slack.com/archives/D096KML3TRV/p1778846087000000) |
| 2026-05-18 | 09:20 | DM Laura | Laura Aguirre | SS invoice/auditoria | Tarea de auditoria/facturas solo autorizada; mover de sprint. | Mantenimiento | Alta | Alonso acepta pasarla al siguiente sprint. | Pendiente | [link](https://singular-innovation.slack.com/archives/D096KML3TRV/p1779114005000000) |
| 2026-05-18 | 10:51 | #ss-internal-team | Miguel Perez | SS Client / Supabase | Confirmar Supabase listo para conexion SS Client al 22. | Mantenimiento | Alta | No se ve cierre en lectura. | Pendiente | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1779119483881939) |
| 2026-05-18 | 11:12 | #ss-internal-team | Esteban Mena | Singular Stories UI | Fix de texto que se sobrepone. | Soporte | Media | Se trabajo en Vercel y ya fue visto. | Resuelto | [link](https://singular-innovation.slack.com/archives/C07FS0AGLTY/p1779120735920519) |
| 2026-05-18 | 13:08 | Grupo Claudia/Alonso/Miguel/Laura | Claudia Galdamez | SS AI wizard | Pasar tarea en ideation al wizard de AI story generator. | Soporte | Media | Alonso propone KP y reconoce que falta flujo. | Pendiente | [link](https://singular-innovation.slack.com/archives/C0B4DKWCC7M/p1779127727000000) |
| 2026-05-18 | 13:00 | DM Camila | Camila Andrea Ruge | Coaching / Google Calendar | Automatizar agenda de coaching con Google Calendar/Make/noreply. | Mantenimiento | Media | Alonso indica que no conoce automatizacion activa y sugiere permisos de Amilkar. | Bloqueado | [link](https://singular-innovation.slack.com/archives/D0ACW67NWGM/p1779127200000000) |

## Pendientes y Riesgos

### Solicitudes sin respuesta o cierre visible

- #ss-internal-team, 2026-05-18: confirmar Supabase listo para SS Client al 22. No se encontro cierre visible.

### Trabajo de soporte/mantenimiento no planificado

- Caso urgente de Gerardo por invoices/metadata consumio varias conversaciones y escalaciones.
- Casos de pagos/estado de talentos y calculo de SPs fueron atendidos como soporte operativo.
- Automatizaciones de Slack duplicadas generaron interrupcion operativa.
- Coordinacion de permisos para Google Calendar dependio de terceros.
