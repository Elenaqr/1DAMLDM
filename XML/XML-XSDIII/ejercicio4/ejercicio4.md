# README - Ejercicio 4: Información de ubicaciones

## Descripción del ejercicio
El ejercicio pide añadir a un XSD existente ("ubicaciones.xsd") la definición de un nuevo tipo complejo llamado "infoUbicacion" que amplíe la definición de "direccion", para validar un documento XML con información adicional sobre ubicaciones.

## Cambios realizados
1. Se definió un nuevo tipo complejo llamado "infoUbicacion"
2. Este nuevo tipo extiende el tipo simple "direccion" existente
3. Se añadió un atributo "metros" de tipo integer
4. Se modificó la referencia de tipo en el elemento "ubicacion" para usar "infoUbicacion" en lugar de "direccion"