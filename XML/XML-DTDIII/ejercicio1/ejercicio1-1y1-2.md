# Ejercicio 1: Cuentos

## Descripción
Este ejercicio tiene 3 archivos:
1. **`ejercicio1-1.xml`**: Información de un cuento con sus personajes y trama.
2. **`ejercicio1-2.xml`**: Información de un cuento con sus personajes y trama.
3. **`ejercicio1-1y1-2.dtd`**: Define la estructura de los archivos XML.

## Estructura del Documento
### `ejercicio1-1.xml` y `ejercicio1-2.xml`
los 2 archivos XML con:
- **cuento**: Elemento raíz con:
  - **Atributos**:
    - `cod`: Código único del cuento (obligatorio).
    - `titulo`: Título del cuento (obligatorio).
  - **Elementos**:
    - **personajes**: Lista de personajes del cuento.
      - **personaje**: Representa un personaje con los siguientes atributos y elementos:
        - **Atributos**:
          - `id`: Identificador único del personaje (obligatorio).
          - `tipo`: Rol del personaje, que puede ser:
            - `principal`: Personaje principal (valor por defecto).
            - `secundario`: Personaje secundario.
            - `antagonista`: Personaje antagonista.
        - **Elementos**:
          - **nombre**: Nombre del personaje.
          - **genero**: Género del personaje.
    - **trama**: Texto que describe la trama del cuento.

### `ejercicio1-1y1-2.dtd`
El archivo DTD define la estructura de los archivos XML:
- **cuento**: Con los elementos `personajes` y `trama`.
- **personajes**: Con 1 o más elementos `personaje`.
- **personaje**: Con los elementos `nombre` y `genero`, y con atributos:
  - `id`: Id del personaje.
  - `tipo`: (`principal`, `secundario`, `antagonista`).
- **nombre**, **genero**, **trama**