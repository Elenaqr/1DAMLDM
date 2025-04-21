# README - Ejercicio 2 de Validación XML con XSD

## Descripción
El ejercicio consiste en crear un XSD (fichas.xsd) para validar un documento XML similar al del Ejercicio 1, pero añadiendo una restricción específica al elemento `edad`.

## Requisitos específicos
- El valor del elemento `edad` debe estar entre 0 y 130 (ambos inclusive)
- Se debe utilizar `xs:minExclusive` en lugar de `xs:minInclusive`
- Se debe utilizar `xs:maxExclusive` en lugar de `xs:maxInclusive`

## Explicación de las restricciones utilizadas
- `xs:minExclusive value="-1"`: Especifica que el valor debe ser mayor que -1 (es decir, 0 o superior)
- `xs:maxExclusive value="131"`: Especifica que el valor debe ser menor que 131 (es decir, 130 o inferior)