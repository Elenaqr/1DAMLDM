# Ejercicio 4-4: Resoluciones

## Descripción
El archivo XML representa una lista de resoluciones de pantalla, el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`resoluciones`**: Elemento raíz con 0 o más elementos `recolucion`.

### Elementos Secundarios
- **`recolucion`**: Cada `recolucion` tiene atributos obligatorios:
  - **`nombre`**: Nombre de la resolución.
  - **`alto`**: Altura de la resolución en píxeles.
  - **`ancho`**: Ancho de la resolución en píxeles.