# Ejercicio 2-5: Reyes Españoles

## Descripción
El archivo XML representa una lista de reyes y reinas españolas el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`reyesEspañoles`**: Elemento raíz que tiene:
  - 0 o más elementos `rey`,`reina`.

### Elementos Secundarios
- **`rey`**: Cada elemento `rey` tiene:
  - **`nombre`**: Nombre del rey.
  - **`padre`**: Nombre del padre del rey.
  - **`madre`**: Nombre de la madre del rey.
- **`reina`**: Cada elemento `reina` tiene:
  - **`nombre`**: Nombre de la reina.
  - **`padre`**: Nombre del padre de la reina.
  - **`madre`**: Nombre de la madre de la reina.