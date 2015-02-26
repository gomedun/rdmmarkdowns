
###Marco Teórico

**BCD:** Un **B**inary **C**oded **D**ecimal es un numero decimal (digitos del 0 al 9) representado en agrupaciones de 4 bits ej. 0001 1000 representa el numero 18.

| Decimal        | BCD           |
| ------------- |-------------:|
| 0 | 0000 |
| 1 | 0001 |
| 2 | 0010 |
| 3 | 0011 |
| 4 | 0100 |
| 5 | 0101 |
| 6 | 0110 |
| 7 | 0111 |
| 8 | 1000 |
| 9 | 1001 |

**Sumador 74ls83:** El 74ls83 es un sumador binario de 4 bits con acarreo, al ser un sumador de binario regular (a diferencia de BCD) este nos permite trabajar con numeros complemento a 2 para llevar a cabo restas.

|   Pin |   Funcion |
|-----  |   -------:|
|   A4-A0 | Bus de entrada del numero A      |
|   B4-B0 | Bus de entrada del numero B     |
|   Σ4-Σ0 | Bits menos significativos de A+B+C0 |
|   C4  | Bit mas significativo de A+B+C0 (quinto bit / salida acarreo) |
|   C0  | Entrada de acarreo |
