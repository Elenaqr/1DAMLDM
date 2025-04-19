# Ejercicio 6: Librería - Documentación XSD

## Descripción del Ejercicio
Este ejercicio requiere un XSD para validar un documento XML que describe una librería con sus datos básicos, información del propietario y un catálogo de libros.

## Requisitos Específicos
1. **Estructura principal:** El elemento `libreria` debe contener:
   - `codigo`: Obligatorio, entero entre 1000 y 9999
   - `direccion`: Obligatorio
   - `telefono`: Obligatorio, 9 dígitos
   - `propietario`: Obligatorio
   - Uno o más elementos `libro`
2. **Elemento propietario:** Contiene:
   - `nombre`: Obligatorio
   - `telefono`: Opcional, puede aparecer múltiples veces, 9 dígitos
3. **Elemento libro:** Contiene:
   - Elementos obligatorios: `titulo`, `autor`, `publicacion`, `precio`
   - Elementos opcionales: `formato`, `cantidad`
4. **Elemento formato:** Valores permitidos: "Rústica", "Tapa blanda", "Tapa dura"
5. **Elemento teléfono:** Debe definirse una vez y reutilizarse en todo el esquema

## Estructura del Esquema XSD
- **Tipos simples personalizados:**
  - `tipoTelefono`: Validación de 9 dígitos para números telefónicos
  - `tipoFormato`: Enumeración de valores permitidos para el formato del libro
- **Tipos complejos personalizados:**
  - `tipoPropietario`: Define la estructura del propietario con nombre y teléfonos
  - `tipoLibro`: Define la estructura de un libro con todos sus elementos
- **Elemento raíz (`libreria`):** Contiene una secuencia de elementos obligatorios y libros
