# Ejercicio 3: Escribir expresiones regulares - Documentación

## Descripción del Ejercicio
Este ejercicio requiere escribir expresiones regulares para XML Schema que satisfagan diferentes patrones de texto. Para cada caso, se deben proporcionar al menos dos soluciones diferentes.

## Soluciones

### 1. "Capítulo 0", "Capítulo 1", "Capítulo 2"... "Capítulo 9" (Solo se permite un dígito)
- **Solución 1:** `Capítulo [0-9]`
- **Solución 2:** `Capítulo \d`

### 2. "Capítulo 0", "Capítulo 1", "Capítulo 2"... "Capítulo 99" (Uno o dos dígitos)
- **Solución 1:** `Capítulo \d{1,2}`
- **Solución 2:** `Capítulo [0-9]{1,2}`
- **Solución 3:** `Capítulo \d|\d\d`

### 3. "Capítulo 1", "Capítulo 2", "Capítulo 3"... "Capítulo 99" (No se permite "Capítulo 0")
- **Solución 1:** `Capítulo [1-9]|\d\d`
- **Solución 2:** `Capítulo [1-9]|[1-9]\d`
- **Solución 3:** `Capítulo [1-9]{1}|\d{2}`

### 4. "Capítulo 0", "Capítulo 1", "Capítulo 2"... "Capítulo 99"... "Capítulo 100"... (Uno o más dígitos)
- **Solución 1:** `Capítulo \d+`
- **Solución 2:** `Capítulo [0-9]+`
- **Solución 3:** `Capítulo \d{1,}`

### 5. Cualquier valor de dos caracteres, cuyo primer carácter sea distinto de un dígito (0-9) y cuyo segundo carácter sea "Z"
- **Solución 1:** `\D[Z]`
- **Solución 2:** `[^\d]Z`
- **Solución 3:** `[^0-9]Z`

### 6. "ABBC", "ABBBC", "ABBBBC", "ABBBBBC"
- **Solución 1:** `AB{2,5}C`
- **Solución 2:** `ABB+C`
- **Solución 3:** `AB{2}|B{3}|B{4}|B{5}C`

### 7. "RSS", "RSSS"... "RSS3"... "RSS8", "RSSS3"... "RSSS8"... "RSSSSSSSSSSS7"...
- **Solución 1:** `RS{2,}[3-8]?`
- **Solución 2:** `RS{2,}|RS{2,}[3-8]`
- **Solución 3:** `RS{2,}([3-8])?`

### 8. "COD645pera", "COD646manzana"...
- **Solución 1:** `COD\d{3}.+`
- **Solución 2:** `COD[0-9]{3}.+`
- **Solución 3:** `COD\d\d\d.{1,}`
