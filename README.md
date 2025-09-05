Calculadora de Factorial
==========================


Descripción


La función factorial calcula el factorial de un número utilizando recursión.


Parámetros


| Nombre | Tipo | Descripción |
| --- | --- | --- |
| n | Entero positivo | El número para calcular factorial |


Valor de retorno


El factorial de n.


Excepciones


* Error si n es negativo.


Ejemplo básico de uso


`javascript
console.log(factorial(5)); // Retorna 120
`


Código fuente


`javascript
/
* Calcula el factorial de un número usando recursión.
*
* @param {number} n El número para calcular factorial (debe ser entero positivo)
* @returns {number} El factorial de n
* @throws {Error} si n es negativo
*/
function factorial(n) {
`


Implementación


`javascript
// Base caso: factorial de 0 o 1 es 1
if (n === 0 || n === 1) {
return 1;
}

// Caso recursivo: factorial de n = n * factorial de (n-1)
else {
return n * factorial(n - 1);
}
}
`


Notas


* Esta función utiliza recursión para calcular el factorial. La recursividad es una técnica común en programación donde un algoritmo se divide en subproblemas más pequeños que son solvidos de manera similar.
* Es importante asegurarse de que la entrada n sea un número entero positivo, ya que el factorial no está definido para números negativos o no enteros.
