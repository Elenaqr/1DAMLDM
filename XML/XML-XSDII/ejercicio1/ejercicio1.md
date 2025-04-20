# Ejercicio 1: Respuestas admitidas - Documentación

## Descripción del Ejercicio
El ejercicio pide explorar diferentes formas de definir una restricción para un elemento `respuesta` que solo acepta como valores las letras "A", "B", "C", "D" o "E".

## Soluciones alternativas usando xs:pattern:

1. **Usando rango de caracteres**:
   <xs:pattern value="[A-E]"/>
   Esta solución aprovecha el hecho de que las letras A, B, C, D y E están en secuencia en el alfabeto, por lo que se pueden representar como un rango.

2. **Usando operador OR (|)**:
   <xs:pattern value="A|B|C|D|E"/>
   Esta solución utiliza | para especificar cada valor permitido de manera individual.

## Parte 2: Alternativa sin usar xs:pattern
Sin usar xs:pattern, podemos lograr la misma restricción utilizando xs:enumeration:

<xs:simpleType>
  <xs:restriction base="xs:string">
    <xs:enumeration value="A"/>
    <xs:enumeration value="B"/>
    <xs:enumeration value="C"/>
    <xs:enumeration value="D"/>
    <xs:enumeration value="E"/>
  </xs:restriction>
</xs:simpleType>
