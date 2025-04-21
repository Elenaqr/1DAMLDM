# README - Ejercicio 3 de Validación XML con XSD

## Descripción
El ejercicio consiste en crear un XSD (precios.xsd) para validar un documento XML que contiene una lista de precios, con restricciones específicas sobre los valores numéricos.

## Requisitos específicos
- Los precios deben tener un máximo de 3 dígitos en total
- De esos dígitos, máximo 2 pueden ser decimales
- La restricción debe ser específica para el elemento `precio` y no reutilizable

## Restricciones utilizadas
- `xs:totalDigits value="3"`: Limita el número total de dígitos (incluyendo decimales) a 3
- `xs:fractionDigits value="2"`: Limita el número de dígitos decimales a 2