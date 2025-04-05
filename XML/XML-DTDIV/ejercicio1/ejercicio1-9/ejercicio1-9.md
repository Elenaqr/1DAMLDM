# Ejercicio 1-9: Sistema Solar

## Descripción
El archivo XML representa un sistema solar utilizando una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`sistemaSolar`**: Elemento raíz que 0 o más elementos `cuerpo`.
- **`cuerpo`**: Cada `cuerpo` tiene:
  - **`planeta`**: Nombre de un planeta (opcional).
  - **`satelite`**: Nombre de un satélite (opcional).
  - **`asteroide`**: Nombre de un asteroide (opcional).