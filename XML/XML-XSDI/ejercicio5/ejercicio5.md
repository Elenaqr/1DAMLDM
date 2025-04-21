# README - Ejercicio 5 de Validación XML con XSD

## Descripción
El ejercicio consiste en corregir un documento XML para que sea válido según un esquema XSD proporcionado.

## Problemas encontrados y correcciones realizadas

1. **Segundo elemento `ficha`**:
   - Problema: El elemento `iniciales` solo contiene dos letras ("MM") cuando el patrón requiere tres letras mayúsculas.
   - Corrección: Se ha cambiado a "MMO" para cumplir con el patrón `[A-Z][A-Z][A-Z]`.

2. **Tercer elemento `ficha`**:
   - Problema: El orden de los elementos no coincide con la secuencia definida en el XSD (`iniciales` aparece antes de `nombre`).
   - Corrección: Se ha reordenado para seguir la secuencia correcta: `nombre`, `iniciales`, `edad`.

3. **Cuarto elemento `ficha`**:
   - Problema 1: El nombre "pablo ruiz picasso" está en minúsculas.
   - Corrección 1: Se ha cambiado a "Pablo Ruiz Picasso" con mayúsculas iniciales.
   - Problema 2: Las iniciales "prp" están en minúsculas cuando el patrón requiere mayúsculas.
   - Corrección 2: Se ha cambiado a "PRP" para cumplir con el patrón.
