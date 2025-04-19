# Ejercicio 3: Heladería 1 - Documentación XSD

## Descripción del Ejercicio
Este ejercicio requiere un XSD para validar un documento XML que describe helados compuestos por combinaciones específicas de sabores, cada uno con una cantidad en gramos y una fecha de fabricación.

## Requisitos Específicos
1. **Primer elemento de helado:** Debe ser `chocolate` o `fresa` (mutuamente excluyentes)
2. **Segundo elemento de helado:** Debe ser `vainilla`, `turron` o `nata`
3. **Contenido de los elementos de sabor:** Cantidad en gramos (entero entre 0 y 1000)
4. **Atributo fabricación:** Debe ser una fecha válida

## Estructura del Esquema XSD
- **Tipo simple personalizado:** `cantidadGramos` para la restricción de valores
- **Elemento raíz (`heladeria`):** Contiene una secuencia de elementos `helado`
  - **Elemento `helado`:**
    - **Atributo `fabricación`:** Tipo fecha
    - **Secuencia de elementos:**
      - **Primera elección (obligatoria):** `chocolate` o `fresa`
      - **Segunda elección (obligatoria):** `vainilla`, `turron` o `nata`