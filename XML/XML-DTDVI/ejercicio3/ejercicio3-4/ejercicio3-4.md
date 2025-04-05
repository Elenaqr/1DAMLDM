# Ejercicio 3-4: Lista de la Compra

## Descripción
El archivo XML representa una lista de la compra,cada elemento de la lista está definido como un elemento `<item>` con atributos obligatorios como el nombre del producto y la cantidad, el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`listaCompra`**: Elemento raíz con 0 o más elementos `item`.

### Elementos Secundarios
- **`item`**: Cada `item` incluye los atributos obligatorios:
  - **`nombre`**: Nombre del producto.
  - **`cantidad`**: Cantidad del producto.