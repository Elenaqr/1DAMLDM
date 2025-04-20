# Ejercicio 4: Letras admitidas - Documentación

## Descripción del Ejercicio
El ejercicio requiere modificar una expresión regular existente para un elemento llamado "letras". En lugar de aceptar 0 o más letras minúsculas, debe aceptar 1 o más pares de letras, donde cada par consiste en una letra mayúscula seguida de una letra minúscula.

### Componentes de la expresión regular:
- `[A-Z]`: Representa cualquier letra mayúscula de la A a la Z
- `[a-z]`: Representa cualquier letra minúscula de la a a la z
- `[A-Z][a-z]`: Representa el patrón de una letra mayúscula seguida de una letra minúscula
- `([A-Z][a-z])+`: Representa uno o más pares de letras, donde cada par es una letra mayúscula seguida de una letra minúscula
