# README - Ejercicio 1: Longitud fija de una clave

## Descripción del ejercicio
El ejercicio pide definir un elemento "clave" que tenga exactamente diez caracteres, los cuales pueden ser letras mayúsculas o minúsculas de la "a" a la "z", o dígitos del "0" al "9".

## Solución 1: Usando xs:pattern y xs:length
<xs:element name="clave">
    <xs:simpleType>
        <xs:restriction base="xs:string">
            <xs:pattern value="[a-zA-Z0-9]*"/>
            <xs:length value="10"/>
        </xs:restriction>
    </xs:simpleType>
</xs:element>
Esta solución combina:
- Un patrón `[a-zA-Z0-9]*` que restringe los caracteres permitidos a letras y números
- La restricción `xs:length value="10"` que exige exactamente 10 caracteres

## Solución 2: Usando únicamente xs:pattern
<xs:element name="clave2">
    <xs:simpleType>
        <xs:restriction base="xs:string">
            <xs:pattern value="[a-zA-Z0-9]{10}"/>
        </xs:restriction>
    </xs:simpleType>
</xs:element>

Esta solución utiliza:
- Un patrón `[a-zA-Z0-9]{10}` que combina la restricción de caracteres con la longitud exacta de 10

## Ejemplos válidos
- "abcde12345"
- "Clave55ABC"
- "1A2b3c4D5f"