# Ejercicio 2: Alumnos 2 - Documentación XSD

## Descripción del Ejercicio
Este ejercicio expande el ejercicio anterior para validar un documento XML que contiene información de múltiples alumnos, con requisitos adicionales sobre la dirección y la provincia.

## Requisitos Específicos
1. **Elemento raíz:** `alumnos` que contiene múltiples elementos `alumno`
2. **Número:** Debe ser un entero en el rango de 0 a 500
3. **Teléfono:** 
   - Debe ser un entero
   - Puede aparecer entre 0 y 5 veces
4. **Dirección:** Puede aparecer 1 o 2 veces
5. **Provincia:** Solo puede contener "Badajoz" o "Cáceres"
6. **Atributo DNI:** Debe seguir el patrón de 8 números seguidos de una letra mayúscula

## Estructura del Esquema XSD
- **Elemento raíz (`alumnos`):** Contiene una secuencia de elementos `alumno`
  - **Elemento `alumno`:** 
    - **Atributo `dni`:** Restricción de patrón para validar el formato
    - **Secuencia de elementos:**
      - `nombre`: Tipo string
      - `direccion`: Tipo complejo con restricciones de ocurrencia (1-2)
        - `calle`: Tipo string
        - `numero`: Tipo entero con restricción de rango
        - `ciudad`: Tipo string
        - `provincia`: Tipo enumeración con valores permitidos
      - `telefono`: Tipo entero con restricciones de ocurrencia (0-5)
