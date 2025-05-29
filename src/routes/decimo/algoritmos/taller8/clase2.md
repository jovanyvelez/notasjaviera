# 24 Ejercicios de Ciclos For y Arrays en C#

**Distribución por grupo:**

    * grupo 1: Ejercicios 1, 2, 3
    * grupo 2: Ejercicios 4, 5, 6
    * grupo 3: Ejercicios 7, 8, 9
    * grupo 4: Ejercicios 10, 11, 12
    * grupo 5: Ejercicios 13, 14, 15
    * grupo 6: Ejercicios 16, 17, 18
    * grupo 7: Ejercicios 19, 20, 21
    * grupo 8: Ejercicios 22, 23, 24

## Ejercicio 1
**Título:** Contador Simple Ascendente

**Enunciado:** Escribe un programa que imprima los números del 1 al 10 en la consola, cada uno en una nueva línea.

**Tips:** Usa un ciclo for que inicialice una variable en 1, continúe mientras sea menor o igual a 10, y se incremente en 1 en cada paso. Dentro del ciclo, usa Console.WriteLine().

---

## Ejercicio 2
**Título:** Contador Simple Descendente

**Enunciado:** Escribe un programa que imprima los números del 10 al 1 en orden descendente, cada uno en una nueva línea.

**Tips:** Usa un ciclo for que inicialice una variable en 10, continúe mientras sea mayor o igual a 1, y se decremente en 1 en cada paso. Dentro del ciclo, usa Console.WriteLine().

---

## Ejercicio 3
**Título:** Números Pares del 1 al 20

**Enunciado:** Escribe un programa que imprima todos los números pares desde el 2 hasta el 20, cada uno en una nueva línea.

**Tips:** Usa un ciclo for que inicialice en 2, continúe mientras sea menor o igual a 20, y se incremente en 2 en cada paso. También puedes usar incremento de 1 y verificar si el número es par con el operador %.

---

## Ejercicio 4
**Título:** Números Impares del 1 al 19

**Enunciado:** Escribe un programa que imprima todos los números impares desde el 1 hasta el 19, cada uno en una nueva línea.

**Tips:** Usa un ciclo for que inicialice en 1, continúe mientras sea menor o igual a 19, y se incremente en 2 en cada paso. También puedes usar incremento de 1 y verificar si el número es impar con el operador %.

---

## Ejercicio 5
**Título:** Tabla de Multiplicar del 5

**Enunciado:** Escribe un programa que imprima la tabla de multiplicar del 5, desde 5x1 hasta 5x10, mostrando el formato "5 x 1 = 5".

**Tips:** Usa un ciclo for del 1 al 10, multiplica cada número por 5 y usa Console.WriteLine() para mostrar el resultado en el formato requerido.

---

## Ejercicio 6
**Título:** Suma de los Primeros 10 Números

**Enunciado:** Escribe un programa que calcule y muestre la suma de los números del 1 al 10.

**Tips:** Inicializa una variable suma en 0, usa un ciclo for del 1 al 10 para sumar cada número a la variable suma, y al final imprime el resultado.

---

## Ejercicio 7
**Título:** Mostrar Elementos de un Array

**Enunciado:** Crea un array con los nombres de 5 frutas y escribe un programa que imprima cada fruta en una línea separada.

**Tips:** Declara un array de strings con 5 frutas, usa un ciclo for con la longitud del array (array.Length) para recorrer todos los elementos y usa Console.WriteLine() para mostrar cada elemento.

---

## Ejercicio 8
**Título:** Contar Elementos de un Array

**Enunciado:** Crea un array con 7 números enteros y escribe un programa que cuente e imprima cuántos elementos tiene el array.

**Tips:** Declara un array de enteros con 7 elementos, usa la propiedad .Length del array para obtener la cantidad de elementos y muestra el resultado con Console.WriteLine().

---

## Ejercicio 9
**Título:** Suma de Elementos de un Array

**Enunciado:** Crea un array con 6 números enteros y escribe un programa que calcule y muestre la suma total de todos los elementos.

**Tips:** Declara un array de enteros, inicializa una variable suma en 0, usa un ciclo for para recorrer el array sumando cada elemento a la variable suma, y muestra el resultado final.

---

## Ejercicio 10
**Título:** Encontrar el Mayor Elemento

**Enunciado:** Crea un array con 5 números enteros y escribe un programa que encuentre y muestre el número mayor del array.

**Tips:** Declara un array de enteros, inicializa una variable mayor con el primer elemento del array, usa un ciclo for para comparar cada elemento con la variable mayor y actualízala si encuentras un número más grande.

---

## Ejercicio 11
**Título:** Contador de Números Pares en Array

**Enunciado:** Crea un array con 8 números enteros y escribe un programa que cuente cuántos números pares hay en el array.

**Tips:** Declara un array de enteros, inicializa un contador en 0, usa un ciclo for para recorrer el array y verifica si cada elemento es par usando el operador %. Incrementa el contador cuando encuentres un número par.

---

## Ejercicio 12
**Título:** Multiplicar Elementos por 2

**Enunciado:** Crea un array con 5 números enteros y escribe un programa que muestre cada elemento multiplicado por 2.

**Tips:** Declara un array de enteros, usa un ciclo for para recorrer el array, multiplica cada elemento por 2 y muestra el resultado con Console.WriteLine().

---

## Ejercicio 13
**Título:** Números del 1 al 15 con Salto

**Enunciado:** Escribe un programa que imprima los números del 1 al 15, pero saltando de 3 en 3 (1, 4, 7, 10, 13).

**Tips:** Usa un ciclo for que inicialice en 1, continúe mientras sea menor o igual a 15, y se incremente en 3 en cada paso. Usa Console.WriteLine() para mostrar cada número.

---

## Ejercicio 14
**Título:** Invertir Array

**Enunciado:** Crea un array con 4 palabras y escribe un programa que las muestre en orden inverso (de la última a la primera).

**Tips:** Declara un array de strings, usa un ciclo for que inicie desde la última posición (array.Length - 1) y decremente hasta llegar a 0. Usa Console.WriteLine() para mostrar cada elemento.

---

## Ejercicio 15
**Título:** Buscar una Palabra

**Enunciado:** Crea un array con 6 nombres de animales y escribe un programa que busque si "gato" está en el array. Muestra "Encontrado" o "No encontrado".

**Tips:** Declara un array de strings con nombres de animales, usa un ciclo for para recorrer el array comparando cada elemento con "gato" usando ==. Usa una variable booleana para recordar si lo encontraste.

---

## Ejercicio 16
**Título:** Promedio de Calificaciones

**Enunciado:** Crea un array con 5 calificaciones (números decimales) y escribe un programa que calcule y muestre el promedio.

**Tips:** Declara un array de tipo double o float, suma todos los elementos usando un ciclo for, divide la suma entre la cantidad de elementos (array.Length) y muestra el resultado.

---

## Ejercicio 17
**Título:** Contar Vocales en Palabras

**Enunciado:** Crea un array con 4 palabras y escribe un programa que cuente cuántas vocales (a, e, i, o, u) hay en total en todas las palabras.

**Tips:** Declara un array de strings, usa un ciclo for para recorrer cada palabra, y dentro otro ciclo para recorrer cada letra. Compara cada letra con las vocales y cuenta las coincidencias.

---

## Ejercicio 18
**Título:** Números Negativos y Positivos

**Enunciado:** Crea un array con 7 números enteros (algunos positivos y algunos negativos) y cuenta cuántos son positivos y cuántos son negativos.

**Tips:** Declara un array con números positivos y negativos, inicializa dos contadores (positivos y negativos), usa un ciclo for para recorrer el array y verifica si cada número es mayor o menor que 0.

---

## Ejercicio 19
**Título:** Tabla de Multiplicar Variable

**Enunciado:** Escribe un programa que muestre la tabla de multiplicar del 3, desde 3x1 hasta 3x12, mostrando el formato "3 x 1 = 3".

**Tips:** Usa un ciclo for del 1 al 12, multiplica cada número por 3 y usa Console.WriteLine() para mostrar el resultado en el formato requerido.

---

## Ejercicio 20
**Título:** Elementos en Posiciones Pares

**Enunciado:** Crea un array con 8 números enteros y escribe un programa que muestre solo los elementos que están en posiciones pares (índices 0, 2, 4, 6).

**Tips:** Declara un array de enteros, usa un ciclo for que incremente de 2 en 2 (i += 2) comenzando desde 0, y muestra los elementos en esas posiciones usando array[i].

---

## Ejercicio 21
**Título:** Factorial de un Número

**Enunciado:** Escribe un programa que calcule el factorial de 5 (5! = 5 x 4 x 3 x 2 x 1).

**Tips:** Inicializa una variable factorial en 1, usa un ciclo for del 1 al 5 multiplicando la variable factorial por cada número del ciclo, y muestra el resultado final.

---

## Ejercicio 22
**Título:** Concatenar Strings de Array

**Enunciado:** Crea un array con 4 palabras y escribe un programa que las una todas en una sola cadena separadas por espacios.

**Tips:** Declara un array de strings, inicializa una variable string vacía, usa un ciclo for para recorrer el array concatenando cada palabra con un espacio a la variable string.

---

## Ejercicio 23
**Título:** Números Múltiplos de 3

**Enunciado:** Escribe un programa que imprima todos los números del 1 al 30 que sean múltiplos de 3.

**Tips:** Usa un ciclo for del 1 al 30, verifica si cada número es múltiplo de 3 usando el operador % (resto de la división). Si el resto es 0, el número es múltiplo de 3.

---

## Ejercicio 24
**Título:** Reemplazar Elementos

**Enunciado:** Crea un array con 6 números enteros y escribe un programa que muestre todos los elementos, pero cambiando los números negativos por 0.

**Tips:** Declara un array con números positivos y negativos, usa un ciclo for para recorrer el array, verifica si cada elemento es menor que 0 y en ese caso muestra 0, sino muestra el elemento original.