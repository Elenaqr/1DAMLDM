# Ejercicio 4-5: Álbumes de Mortadelo

## Descripción
El archivo XML representa una lista de álbumes de Mortadelo, el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`albumesMortadelo`**: Elemento raíz.

### Elementos Secundarios
- **`album`**: Cada `album` tiene atributos obligatorios:
  - **`nombre`**:Nombre del álbum.
  - **`fecha`**: Año de publicación del álbum. Los valores permitidos son: `1969`, `1970`, `1971`, `1972`, `1973`, `1974`.