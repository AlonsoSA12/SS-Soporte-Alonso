# Caso 001 - Ajuste de Performance para Jossy

**Fecha:** 07/04/2026

**Estatus:** Finalizado completo

## Contexto

Alejandra solicito apoyo con una revision de Performance relacionada con Jossy, debido a que la informacion no estaba jalando correctamente. El caso era sensible porque al dia siguiente habia reunion de Performance y se necesitaba que el dato estuviera corregido o, al menos, validado antes de esa sesion.

## Acciones realizadas

Se reviso el origen del dato reportado y se identifico que provenia de la tabla `Weekly Q Performance`. Durante la revision se observo que Jossy aparecia con dos valores fijos, aproximadamente `42K` y `43K`, cuando el valor esperado era `49K`.

Se ingreso a revisar la base de datos, se encontro la formula erronea que estaba generando el descuadre y se ajusto para que los valores cuadraran correctamente. Luego se comunico el cambio a Alejandra para que validara el resultado.

## Resultado

El ajuste quedo corregido. Alejandra valido el resultado y confirmo que estaba correcto.

## Horas hombre invertidas

1.00 HH
