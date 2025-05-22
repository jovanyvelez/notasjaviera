# 16 Ejercicios de C# con Sentencias IF para Principiantes

Estos ejercicios están diseñados para jóvenes de 15-17 años que están comenzando a aprender programación en C#. Cada ejercicio se enfoca en el uso de sentencias `if` y solo requiere conocimientos de tipos de datos básicos (`int`, `double`, `string`) y entrada de datos con `Console.ReadLine()`.

## Ejercicio 1: Verificador de Edad
**Enunciado:** Crea un programa que solicite la edad del usuario y muestre si es mayor de edad (18 años o más) o menor de edad.

**Tips:**
- Usa `Convert.ToInt32()` para convertir la entrada del usuario a un número entero.
- Utiliza un `if` para comparar si la edad es mayor o igual a 18.

## Ejercicio 2: Número Positivo o Negativo
**Enunciado:** Desarrolla un programa que pida al usuario un número y determine si es positivo, negativo o cero.

**Tips:**
- Usa `Convert.ToDouble()` para convertir la entrada a un número que pueda tener decimales.
- Utiliza una estructura `if-else if-else` para verificar las tres condiciones posibles.

## Ejercicio 3: Comparador de Números
**Enunciado:** Crea un programa que solicite dos números y muestre cuál es el mayor o si son iguales.

**Tips:**
- Necesitarás dos variables para almacenar los números ingresados.
- Utiliza una estructura `if-else if-else` para comparar ambos números.

## Ejercicio 4: Calculadora de Descuento
**Enunciado:** Desarrolla un programa que calcule el precio final de un producto con descuento. Si el precio es mayor a 100, aplica un descuento del 10%. Si es mayor a 200, aplica un 15%.

**Tips:**
- Declara una variable para el descuento inicializada en 0.
- Recuerda verificar primero la condición de mayor descuento (precio > 200).
- Calcula el precio final restando el descuento al precio original.

## Ejercicio 5: Verificador de Contraseña
**Enunciado:** Crea un programa que solicite una contraseña y verifique si coincide con una contraseña predefinida (por ejemplo, "secreto123").

**Tips:**
- Define una variable con la contraseña correcta.
- Usa el método `string.Equals()` o el operador `==` para comparar strings.
- Muestra un mensaje diferente según si la contraseña es correcta o incorrecta.

## Ejercicio 6: Clasificador de Notas
**Enunciado:** Desarrolla un programa que solicite una calificación numérica (0-100) y muestre la calificación en letra según esta escala: 
- 90-100: A
- 80-89: B
- 70-79: C
- 60-69: D
- 0-59: F

**Tips:**
- Utiliza una serie de sentencias `if-else if-else` ordenadas de mayor a menor.
- Verifica que la calificación esté dentro del rango válido (0-100).

## Ejercicio 7: Calculadora de IMC
**Enunciado:** Crea un programa que calcule el Índice de Masa Corporal (IMC) de una persona. El usuario debe ingresar su peso (en kg) y altura (en metros). Clasifica el IMC según:
- Menos de 18.5: Bajo peso
- 18.5 - 24.9: Peso normal
- 25 - 29.9: Sobrepeso
- 30 o más: Obesidad

**Tips:**
- La fórmula del IMC es: peso / (altura * altura)
- Usa `Convert.ToDouble()` para ambas entradas.
- Ordena las condiciones desde la mayor a la menor.

## Ejercicio 8: Verificador de Año Bisiesto
**Enunciado:** Desarrolla un programa que determine si un año ingresado por el usuario es bisiesto o no.

**Tips:**
- Un año es bisiesto si es divisible por 4.
- Sin embargo, si el año es divisible por 100, no es bisiesto a menos que también sea divisible por 400.
- Usa el operador `%` (módulo) para verificar si un número es divisible por otro.

## Ejercicio 9: Calculadora Simple
**Enunciado:** Crea una calculadora simple que solicite dos números y una operación (suma, resta, multiplicación o división). Muestra el resultado de la operación elegida.

**Tips:**
- Pide al usuario que ingrese un carácter para la operación ('+', '-', '*', '/').
- Usa un `if` o serie de `if-else` para determinar qué operación realizar.
- Para la división, verifica que el segundo número no sea cero.

## Ejercicio 10: Conversor de Temperatura
**Enunciado:** Desarrolla un programa que convierta entre grados Celsius y Fahrenheit. El usuario debe ingresar la temperatura y la unidad actual, y el programa muestra la conversión.

**Tips:**
- Pide al usuario que indique la unidad con 'C' o 'F'.
- Las fórmulas son: F = C * 9/5 + 32 y C = (F - 32) * 5/9
- Usa una sentencia `if-else` para determinar qué conversión realizar.

## Ejercicio 11: Validador de Triángulo
**Enunciado:** Crea un programa que solicite las longitudes de tres lados y determine si pueden formar un triángulo. Un triángulo es válido si la suma de sus dos lados más cortos es mayor que el lado más largo.

**Tips:**
- Necesitarás comparar las tres combinaciones posibles de lados.
- Usa múltiples condiciones con `&&` (AND lógico).
- Un triángulo también requiere que todos los lados sean positivos.

## Ejercicio 12: Categoría por Edad
**Enunciado:** Desarrolla un programa que clasifique a una persona según su edad en: Niño (0-12), Adolescente (13-17), Adulto (18-64) o Adulto mayor (65+).

**Tips:**
- Usa una estructura `if-else if-else` para las diferentes categorías.
- Verifica primero que la edad sea un número positivo.

## Ejercicio 13: Simulador de Semáforo
**Enunciado:** Crea un programa que simule un semáforo. El usuario ingresa un color (rojo, amarillo o verde) y el programa muestra qué acción debe realizar un conductor (detenerse, precaución o avanzar).

**Tips:**
- Convierte la entrada a minúsculas con `ToLower()` para facilitar la comparación.
- Usa sentencias `if-else if-else` para cada color posible.
- Incluye un caso para cuando el usuario ingrese un color inválido.

## Ejercicio 14: Verificador de Número Par/Impar
**Enunciado:** Desarrolla un programa que determine si un número ingresado por el usuario es par o impar.

**Tips:**
- Un número es par si es divisible por 2 (su residuo al dividir por 2 es 0).
- Usa el operador módulo `%` para verificar la divisibilidad.

## Ejercicio 15: Calculadora de Impuestos
**Enunciado:** Crea un programa que calcule el impuesto sobre un salario según la siguiente escala:
- Hasta 10,000: Sin impuesto
- 10,001 - 25,000: 10% de impuesto
- 25,001 - 50,000: 15% de impuesto
- Más de 50,000: 20% de impuesto

**Tips:**
- Ordena las condiciones de mayor a menor salario.
- Calcula el impuesto multiplicando el salario por el porcentaje correspondiente.
- Muestra tanto el impuesto como el salario neto (salario - impuesto).

## Ejercicio 16: Adivina el Número
**Enunciado:** Desarrolla un juego simple donde el programa "piensa" en un número fijo (por ejemplo, 7) y el usuario debe adivinarlo. El programa da pistas si el número ingresado es mayor, menor o correcto.

**Tips:**
- Define una variable con el número secreto.
- Usa una estructura `if-else if-else` para comparar el número ingresado con el secreto.
- Para hacerlo más interesante en el futuro, podrías generar un número aleatorio, pero eso requiere conocimientos que están fuera del alcance actual.