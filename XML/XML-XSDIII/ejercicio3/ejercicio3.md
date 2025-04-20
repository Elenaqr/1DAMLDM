# README - Ejercicio 3: Precios de artículos

## Descripción del ejercicio
El ejercicio pide modificar un esquema XSD dado ("precios.xsd") para que valide un documento XML diferente que contiene información sobre artículos y sus precios en diferentes monedas. Se debe renombrar el archivo resultante como "articulos.xsd".

### Cambios realizados
1. Se cambió el nombre del elemento raíz de "precios" a "articulos"
2. Se añadió un nivel jerárquico adicional con el elemento "articulo"
3. Se añadió el elemento "nombre" dentro de cada "articulo"
4. Se mantuvo la definición del elemento "precio" con su atributo "moneda"