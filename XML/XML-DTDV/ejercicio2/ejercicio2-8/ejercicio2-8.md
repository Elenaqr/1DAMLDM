# Ejercicio 2-8: Contabilidad

## Descripción
El archivo XML representa un sistema de contabilidad que registra apuntes de ingresos y gastos el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`contabilidad`**: Elemento raíz con 0 o más elementos `apunte`.

### Elementos Secundarios
- **`apunte`**: Cada `apunte` tiene:
  - **`ingreso`**: Opcional.
  - **`gasto`**: Opcional.
  - **`fecha`**: Fecha del apunte.
  - **`cantidad`**: Cantidad asociada al apunte.
  - **`concepto`**: Concepto del apunte.