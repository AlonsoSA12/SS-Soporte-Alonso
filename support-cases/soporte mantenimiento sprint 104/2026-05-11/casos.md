# Casos 2026-05-11

## Caso nro. 15 - Documentacion del fix de approvals unknown

**Detalle o contexto:** Miguel pidio a Alonso explicar que paso con el issue de approvals `unknown` y documentar el fix, porque necesitaba argumentos claros ante una posible escalacion.

**Acciones:**
- Se explico que existian dos flujos de aprobacion: detalle/lista y Sprint View.
- Se identifico que Sprint View no enviaba el email al backend.
- Se documento que el backend guardaba `unknown` cuando no recibia email.
- Se explico que el fix fue volver a enviar el parametro `email`.

**Resultado:**
- Miguel recibio la explicacion tecnica.
- El fix quedo documentado para uso interno.

**Tiempo utilizado:** 0.75 h

## Caso nro. 16 - Talento aparecia como no pagado aunque el sprint ya estaba pagado

**Detalle o contexto:** Alejandra reporto que Carlos Alfredo Martinez Flores aparecia en Singular Stories como no pagado, aunque el pago del sprint ya se habia realizado.

**Acciones:**
- Alonso coordino que Camila tomara el caso por carga de soporte.
- Camila reviso registros en Agile Stories.
- Se reviso revision history y automatizacion de pago.
- Se encontro un espacio final en `Referencia a Proyecto` que rompia el filtro.
- Se corrigio el valor y se actualizaron manualmente las historias afectadas.

**Resultado:**
- Las historias quedaron en estado correcto.
- El caso fue confirmado como resuelto en el grupo.

**Tiempo utilizado:** 1.5 h

## Caso nro. 17 - Lentitud o bloqueo al pasar tareas a in progress

**Detalle o contexto:** Laura reporto por DM que talentos intentaban pasar tareas a `in progress` y la plataforma quedaba pensando o lenta, afectando tambien aprobaciones.

**Acciones:**
- Alonso probo el comportamiento desde su lado.
- Indico que podia ser un problema de Noco/NoLoco o cache.
- Sugirio refrescar o limpiar memoria del navegador.
- Quedo atento a revisar nuevamente despues del deploy.

**Resultado:**
- La prueba local funciono.
- No hay evidencia suficiente de cierre final para todos los talentos.

**Tiempo utilizado:** 0.75 h
