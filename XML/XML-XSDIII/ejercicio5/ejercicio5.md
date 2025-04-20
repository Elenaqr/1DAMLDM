# README - Ejercicio 5: Colores de muebles

## Descripción del ejercicio
El ejercicio pide usar un código XML Schema dado para crear un archivo "muebles.xsd" completo que valide un documento XML con información sobre muebles y sus colores.

## Estructura del esquema completo
1. Se definió un elemento raíz "muebles" que contiene una secuencia de elementos "mueble"
2. Cada elemento "mueble" es del tipo "tipoColorMueble" proporcionado
3. Se mantiene la definición original de los tipos "tipoColorMueble" y "tipoMueble"
4. El tipo "tipoMueble" define los valores permitidos para el contenido (armario, mesa, silla)
5. El tipo "tipoColorMueble" extiende "tipoMueble" añadiendo un atributo "color" con valores permitidos (blanco, gris, negro, wengue)