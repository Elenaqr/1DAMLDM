# Ejercicio 5: FAQ - Documentación XSD

## Descripción del Ejercicio
Este ejercicio requiere un XSD para validar un documento XML que representa un sistema de preguntas frecuentes (FAQ), con información del documento y secciones de preguntas y respuestas.

## Requisitos Específicos
1. **Elemento versión:** Debe seguir el patrón de números, punto, números (e.j. "1.0")
2. **Elemento fecha:** Debe ser un tipo fecha válido
3. **Estructura general:** El elemento `faq` contiene:
   - Exactamente un elemento `info`
   - Uno o más elementos `part`
4. **Elemento info:** Contiene:
   - Elementos obligatorios: `titulo`, `autor`
   - Elementos opcionales: `email`, `version`, `fecha`
5. **Elemento part:** Contiene uno o más elementos `q`
6. **Elemento q:** Contiene los elementos obligatorios `qtext` y `a`

## Estructura del Esquema XSD
- **Tipo simple personalizado:** `tipoVersion` para la validación del formato de versión
- **Tipos complejos personalizados:**
  - `tipoQ`: Define la estructura de una pregunta y respuesta
  - `tipoPart`: Define una sección que contiene múltiples preguntas
  - `tipoInfo`: Define la información del documento FAQ
- **Elemento raíz (`faq`):** Contiene una secuencia de:
  - Un elemento `info` de tipo `tipoInfo`
  - Uno o más elementos `part` de tipo `tipoPart`