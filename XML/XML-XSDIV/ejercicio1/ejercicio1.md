# Ejercicio 1: Alumnos 1 - Documentación XSD

## Descripción del Ejercicio
Este ejercicio requiere un XSD para validar un documento XML que contiene información de un único alumno con su dirección y teléfonos.

## Requisitos Específicos
1. **Elemento raíz:** `alumno` con atributo obligatorio `dni`
2. **Número:** Debe ser un entero en el rango de 0 a 500
3. **Teléfono:** 
   - Debe ser un entero
   - Puede aparecer entre 0 y 5 veces
4. **Atributo DNI:** Debe seguir el patrón de 8 números seguidos de una letra mayúscula

## Estructura del Esquema XSD
- **Elemento raíz (`alumno`):** Define la estructura principal del documento
  - **Atributo `dni`:** Restricción de patrón para validar el formato
  - **Secuencia de elementos:**
    - `nombre`: Tipo string
    - `direccion`: Tipo complejo con estructura anidada
      - `calle`: Tipo string
      - `numero`: Tipo entero con restricción de rango
      - `ciudad`: Tipo string
      - `provincia`: Tipo string
    - `telefono`: Tipo entero con restricciones de ocurrencia
