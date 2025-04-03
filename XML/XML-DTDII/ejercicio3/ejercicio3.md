# Ejercicio 3: Panel de Vuelos

## Descripción
Este ejercicio tiene de 2 archivos:
1. **`ejercicio3.xml`**: _Tiene información sobre un panel de vuelos de un aeropuerto con el nombre del aeropuerto, la fecha y una lista de vuelos con su origen, destino, hora de salida y llegada.
2. **`ejercicio3.dtd`**: Con la estructura del archivo XML.

## Estructura del Documento
### `ejercicio3.xml`
Panel de vuelos con:
- **panel**: Elemento raíz con:
  - **nombre_aeropuerto**: Nombre del aeropuerto.
  - **fecha**: Fecha del panel de vuelos.
  - **vuelos**: Lista de vuelos.
    - **vuelo**: 
      - **Atributos**:
        - `codigo`: Código único del vuelo (obligatorio).
        - `estado`: Estado del vuelo, que puede ser:
          - `C`: Cancelado.
          - `E`: En vuelo.
          - `R`: Retrasado.
      - **Elementos**:
        - **origen**: Ciudad de origen del vuelo.
        - **destino**: Ciudad de destino del vuelo.
        - **salida**: Hora de salida del vuelo.
        - **llegada**: Hora de llegada del vuelo.

### `ejercicio3.dtd`
El archivo DTD define la estructura del archivo XML:
- **panel**: Contiene los elementos `nombre_aeropuerto`, `fecha` y `vuelos`.
- **vuelos**: Contiene uno o más elementos `vuelo`.
- **vuelo**: Incluye los elementos `origen`, `destino`, `salida` y `llegada`, y tiene los atributos:
  - `codigo`: Identificador único del vuelo.
  - `estado`: Estado del vuelo (`C`, `E`, `R`).
- **origen**, **destino**, **salida**, **llegada**: Contienen datos de texto (`#PCDATA`).
