# Ejercicio 2: Números y letras - Documentación

## Descripción del Ejercicio
El ejercicio requiere crear un XSD para validar un documento XML que contiene una colección de fichas.

## Requisitos Específicos
1. **Elemento raíz:** `fichas` que contiene múltiples elementos `ficha`
2. **Atributo `numero` y elemento `codigo`:**
   - Ambos deben usar la misma restricción
   - Solo pueden contener un valor entero de dos dígitos entre "00" y "19"
3. **Atributo `letra`:**
   - Solo puede tomar los valores "X", "Y" o "Z"
   - La restricción debe ser usada exclusivamente por este atributo
   - Es opcional (puede no aparecer)
4. **Atributo `numero`:**
   - Es obligatorio para cada ficha