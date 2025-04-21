# README - Ejercicio 4 de Validación XML con XSD

## Descripción
El ejercicio consiste en redefinir un elemento `vehiculo` y crear un tipo simple reutilizable para la restricción que limita los valores a una enumeración específica.

## Problema original
En la definición original, se crea un elemento `vehiculo` con un tipo simple anónimo que restringe los valores a: "barco", "bicicleta", "coche" y "tren".

## Solución
Se ha creado:
1. Un tipo simple nombrado `tipoDeVehiculo` con la restricción de enumeración
2. El elemento `vehiculo` que utiliza este tipo
3. Un ejemplo adicional de elemento `transporte` que también utiliza el mismo tipo
