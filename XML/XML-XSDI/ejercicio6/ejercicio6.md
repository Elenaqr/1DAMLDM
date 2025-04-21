# README - Ejercicio 6 de Validación XML con XSD

## Descripción
El ejercicio consiste en modificar un esquema XSD existente para que admita un nuevo elemento `iniciales-al-reves` que debe compartir el mismo tipo que el elemento `iniciales`.

## Requisitos específicos
1. Añadir el nuevo elemento `iniciales-al-reves` al esquema
2. Usar el mismo tipo de datos para `iniciales` e `iniciales-al-reves`
3. Definir el tipo solo una vez para que sea reutilizable

## Cambios realizados
1. Se ha creado un tipo simple nombrado `tipoIniciales` con la restricción de patrón `[A-Z][A-Z][A-Z]`
2. Se ha modificado la definición del elemento `iniciales` para usar este tipo
3. Se ha añadido el elemento `iniciales-al-reves` usando el mismo tipo