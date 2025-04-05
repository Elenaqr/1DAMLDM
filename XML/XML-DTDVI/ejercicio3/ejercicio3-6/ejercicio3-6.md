# Ejercicio 3-6: Fútbol

## Descripción
El archivo XML representa una lista de jugadores de fútbol y equipos, el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`futbol`**: Elemento raíz con 0 o más elementos `jugador` o `equipo`.

### Elementos Secundarios
- **`jugador`**: Cada elemento `jugador`tiene atributos obligatorios:
  - **`nombre`**: Atributo con el nombre del jugador y se debe escribir sin espacios ni caracteres especiales.
  - **`codigo`**: Atributo con un identificador único para el jugador.

- **`equipo`**: Cada `equipo` tiene atributos:
  - **`nombre`**: Nombre del equipo.
  - **`jugadores`**: Lista de referencias a los códigos de los jugadores que pertenecen al equipo.