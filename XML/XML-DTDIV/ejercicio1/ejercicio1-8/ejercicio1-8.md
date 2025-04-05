# Ejercicio 1-8: Agenda de Contactos

## Descripción
El archivo XML representa una agenda de contactos utilizando una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`agenda`**: Elemento raíz con 0 o más elementos `contacto`.
- **`contacto`**: Cada `contacto` tiene:
  - **`nombre`**: Nombre del contacto.
  - **`telefonoFijo`**: 0 o más números de teléfono fijo.
  - **`telefonoMovil`**: 1 o más números de teléfono móvil.
