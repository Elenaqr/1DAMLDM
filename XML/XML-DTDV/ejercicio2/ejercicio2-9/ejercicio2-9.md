# Ejercicio 2-9: Mensajes

## Descripción
El archivo XML representa una lista de mensajes intercambiados entre usuarios el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`mensajes`**: Elemento raíz con 0 o más elementos `mensaje`.

### Elementos Secundarios
- **`mensaje`**: Cada `mensaje` tiene:
  - **`de`**: Remitente del mensaje.
  - **`para`**: Destinatario del mensaje.
  - **`hora`**: Hora en la que se envió el mensaje.
  - **`texto`**: Contenido del mensaje.
  - **`strong`**: Elemento opcional dentro de `texto`.