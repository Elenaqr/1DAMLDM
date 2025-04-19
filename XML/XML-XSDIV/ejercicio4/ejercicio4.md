# Ejercicio 4: Heladería 2 - Documentación XSD

## Descripción del Ejercicio
Este ejercicio requiere un XSD para validar un documento XML que describe helados compuestos únicamente por combinaciones específicas de sabores, donde los sabores son elementos vacíos.

## Requisitos Específicos
1. **Combinaciones permitidas:** El helado solo puede ser:
   - `fresa` y `chocolate`, o
   - `vainilla` y `chocolate`
2. **Elementos de sabor:** Sin contenido

## Estructura del Esquema XSD
- **Elemento raíz (`heladeria`):** Contiene una secuencia de elementos `helado`
  - **Elemento `helado`:** Contiene una elección entre:
    - **Opción 1:** Secuencia de elementos vacíos `fresa` y `chocolate`
    - **Opción 2:** Secuencia de elementos vacíos `vainilla` y `chocolate`
