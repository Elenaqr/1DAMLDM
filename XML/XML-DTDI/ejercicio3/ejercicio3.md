# Ejercicio 3: Agenda Personal

## Descripción
Este ejercicio tiene de 2 archivos:
1. **`ejercicio3.xml`**: Con la información personal de una persona, como su nombre, apellidos, teléfono, fecha de nacimiento y lugar de nacimiento.
2. **`ejercicio3.dtd`**: Define la estructura del archivo XML.

## Archivos
### `ejercicio3.xml`
El XML describe una agenda personal con:
- **agenda**: Elemento raíz.
  - **nombre**: Nombre de la persona.
  - **apellido**: Apellidos de la persona (puede haber 1 o más).
  - **telefono**: Número de teléfono de la persona.
  - **fecha_nacimiento**: Fecha de nacimiento, dividida en:
    - **anio**: Año de nacimiento.
    - **mes**: Mes de nacimiento.
    - **dia**: Día de nacimiento.
  - **lugar_nacimiento**: Lugar de nacimiento, dividido en:
    - **pais**: País de nacimiento.
    - **ciudad**: Ciudad de nacimiento.
    - **localidad**: Localidad de nacimiento.

### `ejercicio3.dtd`
Este archivo DTD define la estructura del archivo XML:
- **agenda**: Con elementos `nombre`, `apellido+`, `telefono`, `fecha_nacimiento` y `lugar_nacimiento`.
- **fecha_nacimiento**: Con los elementos `anio`, `mes` y `dia`.
- **lugar_nacimiento**: Con los elementos `pais`, `ciudad` y `localidad`.

