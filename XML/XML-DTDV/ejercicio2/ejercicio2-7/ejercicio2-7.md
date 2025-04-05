# Ejercicio 2-7: Colores

## Descripción
El archivo XML representa una lista de colores el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`colores`**: Elemento raíz que con 0 o más elementos `color`.

### Elementos Secundarios
- **`color`**: Cada elemento `color` tiene:
  - **`nombreSvg`**: Nombre del color.
  - **`codigo`**: Código del color, puede estar en RGB o CMYK.
- **`codigo`**: Cada `codigo` tiene:
  - **`rgb`**: Código en formato RGB.
  - **`cmyk`**: Código en formato CMYK.