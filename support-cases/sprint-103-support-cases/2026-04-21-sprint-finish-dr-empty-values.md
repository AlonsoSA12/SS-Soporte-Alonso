# Caso 001 - Sprint Finish y DR vacios por falta de Impact Level

**Fecha:** 21/04/2026

**Estatus:** Finalizado completo

## Contexto

Laura reporto que los campos `Sprint Finish` y `DR` le estaban llegando vacios. Durante una llamada de revision se validaron los campos afectados y se identifico que el comportamiento estaba relacionado con la forma en que se alimentaban `Sprint Finish` y `Sprint Order`.

## Acciones realizadas

Se reviso junto con Laura cuales eran los campos impactados y se confirmo que el problema estaba en `Sprint Finish` y `Sprint Order`. Luego se reviso la configuracion del campo y el prompting asociado, donde se identifico que el recurso utilizado para completar esos valores era el `Impact Level` de cada tarea.

Durante la validacion se detecto que las tareas de Laura no tenian `Impact Level` asignado. Laura realizo la asignacion correspondiente y, despues de eso, se volvio a probar el flujo para confirmar el resultado.

## Resultado

Una vez asignado el `Impact Level` en las tareas, los campos comenzaron a completarse correctamente y el caso quedo resuelto.

## Horas hombre invertidas

0.50 HH
