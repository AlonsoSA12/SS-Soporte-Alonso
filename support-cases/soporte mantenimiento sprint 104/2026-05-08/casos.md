# Casos 2026-05-08

## Caso nro. 10 - Permiso para impersonar usuario en Singular Stories

**Detalle o contexto:** Miguel reporto por DM que Alejandra no podia impersonar a otro usuario en Singular Stories. El bloqueo afectaba una revision operativa del caso de contabilidad.

**Acciones:**
- Se reviso el correo asociado.
- Se valido el proyecto y estado del usuario.
- Se ajusto el acceso necesario para impersonar.

**Resultado:**
- El acceso quedo corregido para el caso reportado.
- Alonso confirmo el proyecto en Estimation.

**Tiempo utilizado:** 0.5 h

## Caso nro. 11 - Investigacion de metadata incorrecta en aprobaciones

**Detalle o contexto:** Miguel reporto en `#review-invoice` un issue de metadata en aprobaciones, donde algunas aprobaciones aparecian con datos incorrectos o `unknown`.

**Acciones:**
- Se revisaron registros disponibles.
- Se evaluo si Pipedream o N8N guardaban historial suficiente.
- Se comenzo a buscar trazabilidad por fecha, hora y usuario.

**Resultado:**
- Se confirmo que existian limitaciones de retencion.
- El caso quedo parcialmente resuelto y conectado al fix de Sprint View.

**Tiempo utilizado:** 1.5 h

## Caso nro. 12 - Fix de aprobacion masiva que guardaba email como unknown

**Detalle o contexto:** En DM con Miguel, Alonso identifico que la aprobacion masiva desde Sprint View no enviaba el email al backend. Por eso la metadata de confirmacion quedaba como `unknown`.

**Acciones:**
- Se compararon los flujos de aprobacion individual y aprobacion masiva.
- Se detecto que el boton de Sprint View no enviaba el parametro `email`.
- Se agrego nuevamente el email al request.
- Se documento la causa para que Miguel tuviera argumentos ante posible escalacion.

**Resultado:**
- El flujo quedo corregido hacia adelante.
- El historico con `unknown` no quedo totalmente recuperable por falta de datos persistidos.

**Tiempo utilizado:** 2.0 h

## Caso nro. 13 - Busqueda de logs en N8N, Pipedream y PostHog

**Detalle o contexto:** Para recuperar evidencia de aprobaciones, Alonso consulto fuentes de trazabilidad en N8N, Pipedream y PostHog con apoyo de Luis, Claudia y Camila.

**Acciones:**
- Se consulto si N8N conservaba historial de ejecuciones antiguas.
- Se valido retencion de Pipedream por plan.
- Se pidio acceso a PostHog y recordings.
- Se reviso si era posible cruzar fecha/hora con sesiones de usuario.

**Resultado:**
- N8N community borra historial diario por default.
- Pipedream/PostHog tienen retencion limitada.
- La recuperacion completa quedo bloqueada por disponibilidad de logs.

**Tiempo utilizado:** 1.5 h

## Caso nro. 14 - Reporte de aprobaciones para ultimos sprints

**Detalle o contexto:** Gerardo pidio reporte de los ultimos 3 sprints con historias aprobadas porque tenia facturas frenadas y necesitaba comprobar aprobaciones.

**Acciones:**
- Se revisaron historias aprobadas por sprint.
- Se identificaron casos con correo conocido y casos `unknown`.
- Se preparo reporte por fechas.
- Se compartio video explicativo para entender el problema.

**Resultado:**
- Se entrego un pre-reporte/video para soporte de decision.
- Algunos casos quedaron sin identificacion completa por falta de fuente recuperable.

**Tiempo utilizado:** 2.0 h
