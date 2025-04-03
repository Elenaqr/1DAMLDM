# Ejercicio 2: Equipos de la NBA

## Descripción
Equipos de la NBAcon el nombre del equipo, la conferencia a la que pertenece, el número de títulos ganados, su posición en la clasificación y su quinteto titular. Utiliza una DTD interna.

## Estructura del Documento
La estructura:
- **EquiposNBA**: Elemento raíz.
  - **equipo**: Equipo de la NBA con:
    - **Atributos**:
      - `conferencia`:"Este" o "Oeste" (obligatorio).
    - **Elementos**:
      - **nombre**: Nombre del equipo.
      - **titulos**: Número de títulos ganados por el equipo.
      - **posicion**: Posición del equipo en la clasificación.
      - **quinteto**: Quinteto titular del equipo.
