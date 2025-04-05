# Ejercicio 4-3: Cosas por Hacer

## Descripción
El archivo XML representa una lista de tareas o cosas por hacer, el documento está definida por una DTD interna.

## Estructura del Documento
### Elemento Principal
- **`cosasPorHacer`**: Elemento raíz.

### Elementos Secundarios
- **`cosa`**: Cada `cosa` tiene atributos obligatorios:
  - **`fecha`**:Tiene la fecha en la que se registró la tarea.
  - **`asunto`**:Describe el asunto de la tarea.
  - **`fechaLimite`**: Indica la fecha límite para completar la tarea.