### Nota General: Recuerda que para leer un número ingresado por el usuario como texto y usarlo en cálculos, necesitarás convertirlo. Puedes usar Convert.ToInt32(Console.ReadLine()).

 1. **Titulo: Contador Simple Ascendente**

    **Enunciado**: Escribe un programa que imprima los números del 1 al 10 en la consola, cada uno en una nueva línea.
    
    **Tips**: Usa un ciclo for que inicialice una variable en 1, continúe mientras sea menor o igual a 10, y se incremente en 1 en cada paso. Dentro del ciclo, usa Console.WriteLine().


2. **Titulo: Cuenta Regresiva**

    **Enunciado**: Escribe un programa que imprima los números del 10 al 1 en la consola, cada uno en una nueva línea.
    
    **Tips**: Similar al anterior, pero el ciclo for deberá inicializar la variable en 10, continuar mientras sea mayor o igual a 1, y decrementarse en 1.


3. **Titulo: Contador Hasta N**

    **Enunciado**: Pide al usuario un número entero positivo N. Luego, imprime los números del 1 hasta N.
    
    **Tips**: Primero, solicita el número usando Console.ReadLine() y conviértelo con Convert.ToInt32(). El ciclo for usará N como su límite superior.


4. **Titulo: Números Pares hasta 20**
    
    **Enunciado**: Escribe un programa que imprima todos los números pares desde el 2 hasta el 20.
    
    **Tips**: Puedes hacer que tu variable de control en el for se incremente de 2 en 2. O bien, usa un if dentro del ciclo for (que va de 1 a 20) y el operador módulo (%) para verificar si un número es par (numero % 2 == 0).


5.  **Titulo: Suma de los Primeros N Números**
    
    **Enunciado**: Pide al usuario un número entero N. Calcula y muestra la suma de todos los números desde 1 hasta N (ej: si N=3, suma=1+2+3=6).
    
    **Tips**: Necesitarás una variable acumuladora (ej: sumaTotal) inicializada en 0 antes del ciclo for. Dentro del ciclo, suma el valor actual del contador a sumaTotal.


6. **Titulo: Tabla de Multiplicar**

    **Enunciado**: Pide al usuario un número entero. Luego, muestra la tabla de multiplicar de ese número, del 1 al 10 (ej: si ingresa 5, mostrar 5x1=5, 5x2=10, ..., 5x10=50).
    
    **Tips**: El ciclo for irá del 1 al 10. Dentro del ciclo, multiplica el número ingresado por el contador del ciclo y muestra el resultado.

7. **Titulo: Factorial de un Número**
   
   **Enunciado**: Pide al usuario un número entero no negativo N. Calcula y muestra su factorial (N!). Recuerda que 0! = 1.
   
   **Tips**: Necesitarás una variable para el resultado (ej: factorial) inicializada en 1. El ciclo for puede ir desde 1 hasta N. En cada paso, multiplica factorial por el contador del ciclo. Considera el caso especial de N=0 con un if antes del ciclo.


8. **Titulo: Repetidor de Mensajes**

   **Enunciado**: Pide al usuario un mensaje (texto) y un número N. Luego, muestra el mensaje N veces en la consola.

   **Tips**: Lee el mensaje con Console.ReadLine(). Lee el número N y conviértelo. El ciclo for se ejecutará N veces, y en cada iteración imprimirá el mensaje.


9.  **Titulo: Promedio de 5 Calificaciones**

    **Enunciado**: Pide al usuario que ingrese 5 calificaciones (una por una). Al final, calcula y muestra el promedio de estas calificaciones.

    **Tips**: Usa un ciclo for que se repita 5 veces. Dentro del ciclo, pide una calificación, conviértela y súmala a una variable acumuladora. Después del ciclo, divide la suma total entre 5.


10. **Titulo: Dibujando una Línea Horizontal**

    **Enunciado**: Pide al usuario un número N. Dibuja una línea horizontal de N asteriscos (*).

    **Tips**: Usa un ciclo for que se repita N veces. Dentro del ciclo, usa Console.Write("*") (sin Line) para que los asteriscos se impriman en la misma línea. Después del ciclo, puedes usar Console.WriteLine() para mover el cursor a la siguiente línea.


11. **Titulo: Números Impares hasta N**

    **Enunciado**: Pide al usuario un número N. Imprime todos los números impares desde 1 hasta N.

    **Tips**: Usa un ciclo for desde 1 hasta N. Dentro del ciclo, usa un if y el operador módulo (%) para verificar si el número actual es impar (numero % 2 != 0).


12. **Titulo: Adivina el Número Secreto (Simplificado)**

    **Enunciado**: Define un número secreto (ej: 7). Dale al usuario 3 intentos para adivinarlo. En cada intento, dile si acertó o no.

    **Tips**: Usa un for que se repita 3 veces. Dentro, pide un número al usuario. Usa un if para comparar con el número secreto. Si acierta, puedes usar break; para salir del ciclo.


13. **Titulo: Contador con Saltos**

    **Enunciado**: Pide al usuario un número inicial, un número final y un tamaño de ***salto***. Imprime los números desde el inicial hasta el final, incrementando según el salto.

    **Tips**: El for se inicializará con numeroInicial, la condición será variable ***menor o igual*** numeroFinal, y el incremento será variable += salto.


14. **Titulo: Lista de Nombres Numerada**
    
    **Enunciado**: Pide al usuario cuántos nombres quiere ingresar (N). Luego, pide cada uno de los N nombres y muéstralos como una lista numerada (ej: 1. Ana, 2. Luis, 3. Carlos).

    **Tips**: El ciclo for irá de 1 a N. Dentro del ciclo, lee un nombre. Imprime el valor del contador del ciclo, un punto, un espacio y el nombre.


15. **Titulo: Caracteres de una Palabra**

    **Enunciado**: Pide al usuario una palabra. Imprime cada carácter de la palabra en una línea separada.

    **Tips**: Lee la palabra. Un ciclo for puede ir desde 0 hasta palabra.Length - 1. Para acceder a cada carácter, usa palabra[i], donde i es el contador del ciclo.

16. **Titulo: ¿Es Mayor de Edad? (Múltiples Personas)**

    **Enunciado**: Pregunta la edad a 3 personas diferentes. Para cada persona, indica si es mayor de edad (considera 18 años o más) o no.

    **Tips**: Usa un ciclo for que se repita 3 veces. Dentro del ciclo: pide la edad, conviértela, y usa un if para determinar si edad >= 18. Muestra el mensaje correspondiente.


17. **Titulo: Suma de Pares en un Rango**

    **Enunciado**: Pide al usuario dos números, inicio y fin. Calcula y muestra la suma de todos los números pares dentro de ese rango (incluyendo inicio y fin si son pares).

    **Tips**: Usa un for que vaya de inicio a fin. Dentro, con un if y el operador módulo (%), verifica si el número actual es par. Si lo es, súmalo a un acumulador.


18. **Titulo: FizzBuzz Básico**

    **Enunciado**: Imprime los números del 1 al 30. Pero:
    Si el número es divisible por 3, imprime "Fizz".
    Si el número es divisible por 5, imprime "Buzz".
    Si es divisible por ambos (3 y 5), imprime "FizzBuzz".
    Si no, imprime el número.

    **Tips**: Usa un for del 1 al 30. Dentro, usa una cadena de if-else if-else. ¡El orden de las condiciones importa! Verifica "FizzBuzz" (divisible por 3 Y por 5) primero.


19. **Titulo: Invertir una Cadena Corta**

    **Enunciado**: Pide al usuario una palabra de máximo 5 letras. Imprime la palabra invertida. (Ej: "hola" -> "aloh").

    **Tips**: Lee la palabra. Un ciclo for puede recorrer la palabra desde el último carácter (palabra.Length - 1) hasta el primero (0), decrementando. Ve concatenando cada carácter a una nueva cadena.


20. **Titulo: Potencias de 2**

    **Enunciado**: Imprime las primeras 8 potencias de 2 (desde 2^0 hasta 2^7).

    **Tips**: Puedes usar un for de 0 a 7. Dentro del ciclo, calcula Math.Pow(2, contadorDelCiclo). O bien, mantén una variable que se multiplica por 2 en cada iteración.


21. **Titulo: Ahorro Mensual Fijo**

    **Enunciado**: Una persona decide ahorrar $100 cada mes durante un año (12 meses). Muestra cuánto dinero ha ahorrado al final de cada mes.

    **Tips**: Usa un for que represente los meses (de 1 a 12). Necesitarás una variable ahorroTotal inicializada en 0. En cada iteración, suma 100 a ahorroTotal y muestra el ahorroTotal de ese mes.


22. **Titulo: Contador de Vocales 'a'**

    **Enunciado**: Pide al usuario una frase. Cuenta cuántas veces aparece la vocal 'a' (minúscula) en la frase.

    **Tips**: Lee la frase. Usa un for para recorrer cada carácter de la frase (frase.Length). Dentro, con un if, compara si frase[i] == 'a'. Lleva la cuenta en una variable.


23. **Titulo: Múltiplos de 7 hasta 70**

    **Enunciado**: Imprime todos los múltiplos de 7, desde 7 hasta 70.

    **Tips**: Puedes hacer un for que empiece en 7, termine en 70, y se incremente de 7 en 7.


24. **Titulo: Simulador de Crecimiento de Planta**

    **Enunciado**: Una planta crece 2 cm cada día durante 5 días. Muestra la altura de la planta al final de cada día, asumiendo que empieza con 0 cm.

    **Tips**: Usa un for que se repita 5 veces (días). Mantén una variable altura inicializada en 0. En cada día, incrementa altura en 2 y muestra la altura actual.




 