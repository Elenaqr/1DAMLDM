# Ejercicio 2: Liga de Baloncesto

## Descripción
Este ejercicio está compuesto de 2 archivos:
1. **`ejercicio2.xml`**: Contiene información sobre una liga de baloncesto, incluyendo jugadores, sus equipos y detalles adicionales.
2. **`ejercicio2.dtd`**: Define la estructura del archivo XML¡.

## Archivos
### `ejercicio2.xml`
El XML trata sobre una liga de baloncesto con:
- **liga_baloncesto**: Elemento raíz.
- **jugador**: El jugador con los siguientes datos:
  - **nombre**: Nombre del jugador.
  - **apellidos**: Apellidos del jugador.
  - **equipo**: Información sobre el equipo del jugador:
    - **ciudad**: Ciudad del equipo.
    - **presidente**: Detalles del presidente del equipo:
      - **nombrePresidente**: Nombre del presidente.
      - **apellidosPresidente**: Apellidos del presidente.
  - **edad**: Edad del jugador.

### `ejercicio2.dtd`
Archivo DTD con la estructura del archivo XML:
- **liga_baloncesto**: 1 o más elementos `jugador`.
- **jugador**: Elementos `nombre`, `apellidos`, `equipo` y `edad`.
- **equipo**: Elementos `ciudad` y `presidente`.
- **presidente**: Elementos `nombrePresidente` y `apellidosPresidente`.
