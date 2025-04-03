# Ejercicio 1: Factura

## Descripción
Factura que incluye información sobre el emisor, el cliente y el detalle de los artículos facturados. Utiliza una DTD interna con la estructura del documento.

## Estructura del Documento

### Elementos Principales
- **factura**: Elemento raíz.
  - **Atributos**:
    - `numero`: Número único de la factura (obligatorio).
    - `fecha`: Fecha de emisión de la factura (obligatorio).

- **datos_emisor**: Información del emisor de la factura.
  - **nombre**: Nombre del emisor.
  - **cif**: Código de Identificación Fiscal (CIF) del emisor.
  - **telefono**: Teléfono de contacto del emisor.

- **datos_cliente**: Información del cliente.
  - **nombre**: Nombre del cliente.
  - **cif**: Código de Identificación Fiscal (CIF) del cliente.
  - **telefono**: Teléfono de contacto del cliente.

- **detalle_factura**: Detalle de los artículos facturados.
  - **Atributos**:
     - `importe`
