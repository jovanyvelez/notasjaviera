# ¡Hey, Parceros y Parceras Programadoras de Medallo! 🚀

¡Qué más pues! Bienvenidos a esta nueva aventura donde vamos a aprender unos trucos súper poderosos para que sus programas hagan cosas increíbles. Hoy vamos a hablar de **Ciclos** y **Arreglos**. Suena como a cosa de nerds, ¿cierto? ¡Pero qué va! Es más fácil de lo que creen y les va a servir pa' un montón de cosas, desde organizar la música de su celular hasta crear sus propios juegos.

Imaginen que van a hacer un sancocho bien delicioso pa' invitar a todo el combo de amigos. Hay tareas que se repiten, ¿o qué? Como picar la yuca, la papa, el plátano... ¡Uff! Y también necesitan una lista de todos los ingredientes pa' que no se les olvide nada. Bueno, los ciclos y los arreglos nos ayudan con eso en el mundo de la programación.

**¿Listos pa' poner al computador a camellar por ustedes?** ¡Empecemos!

---

## ⚙️ ¿Qué Son los Ciclos? - Poniendo al Computador a "Camellar" por Vos

En la vida real, hay muchas cosas que hacemos una y otra vez.
*   Escuchar esa canción de Feid o Karol G que no se les sale de la cabeza... ¡en bucle!
*   Darle vueltas a la cancha de fútbol del barrio pa' calentar.
*   Cuando la abuela les dice: "Mijo, salúdeme a toda la familia", y ustedes empiezan: "Hola tía...", "Hola primo...", y así con cada uno.

Bueno, en programación, un **ciclo** (o bucle) es simplemente una forma de decirle al computador: "¡Parcero, repetí esta tarea varias veces!". Así no tenemos que escribir el mismo código mil veces. ¡El computador lo hace por nosotros!

Hay dos tipos principales de ciclos que vamos a ver, como tener dos rutas distintas pa' llegar al Poblado: el ciclo `for` y el ciclo `while`.

---

### 🔁 El Ciclo `for`: Cuando Sabés Cuántas Vueltas Dar

El ciclo `for` es el que usamos cuando sabemos **exactamente cuántas veces** queremos que se repita algo. Es como cuando el profe de educación física dice: "¡Cinco vueltas a la cancha, pues!". Sabés que son 5, ni más ni menos.

**Piénsenlo así:**

*   Quieren enviar un mensaje de "Feliz Navidad, parcero" a sus 10 mejores amigos. Saben que son 10 mensajes.
*   Quieren contar los pisos de un edificio que tiene 20 pisos.

**¿Cómo se ve esto en C#?**

La estructura básica es como una orden con tres partes:

**for** (**dónde empezamos a contar**; ***hasta cuándo contamos***; ***cómo avanzamos en el conteo***)

```csharp
/*  Imaginen que quieren saludar 5 veces, 
    ¡como los goles de su equipo favorito!
*/
// i empieza en 1; 
// se repite mientras i sea menor o igual a 5; 
// i aumenta de 1 en 1
for (int i = 1; i <= 5; i++) 
{
    Console.WriteLine("¡Hola, futuro programador de Medallo! Saludo número: " + i);
}
```

**Resultado en la consola:**
```
¡Hola, futuro programador de Medallo! Saludo número: 1
¡Hola, futuro programador de Medallo! Saludo número: 2
¡Hola, futuro programador de Medallo! Saludo número: 3
¡Hola, futuro programador de Medallo! Saludo número: 4
¡Hola, futuro programador de Medallo! Saludo número: 5
```

**Ejemplo bien paisa con `for`:**

Vamos a simular que estamos anunciando las estaciones de la Línea A del Metro, desde Niquía hasta La Estrella (vamos a poner solo algunas pa' no alargar mucho).

```csharp
// Algunas estaciones principales de la Línea A del Metro
string[] estacionesMetro = {"Niquía", "Bello", "Madera", "Acevedo", "Caribe", "San Antonio", "Poblado", "Envigado", "Itagüí", "La Estrella"};

Console.WriteLine("--- Recorrido Línea A del Metro (Norte a Sur) ---");
for (int i = 0; i < 10; i++) // Sabemos que queremos mostrar 10 estaciones en este ejemplo
{
    // Más adelante veremos cómo usar el nombre de la estación directamente del arreglo ;)
    Console.WriteLine("Próxima estación: ... (anunciando parada " + (i + 1) + ")");
}
```
*(Más adelante, cuando veamos arreglos, haremos este ejemplo del Metro mucho más bacano).*

---

### 🔄 El Ciclo `while`: Mientras Haya Aguardiente en la Botella... (¡O se Cumpla una Condición!)

Ahora, el ciclo `while` es diferente. Este lo usamos cuando queremos que algo se repita **mientras una condición sea verdadera**, pero no sabemos exactamente cuántas veces va a ser.

**Piénsenlo así:**

*   Jugar parqués hasta que alguien gane. ¿Cuántas rondas serán? ¡Quién sabe! Se juega *mientras* nadie haya ganado.
*   Comer empanadas en la esquina hasta que se llenen. ¿Cuántas se van a comer? Depende del hambre, ¿cierto? Comen *mientras* todavía tengan hambre (y plata).
*   Buscar वाई-फाई en el celular hasta que se conecte.

**¿Cómo se ve esto en C#?**

La estructura es más sencilla:
`while (esta condición sea verdadera)`

```csharp
// Juego simple: Adivinar un número que la "comPU" pensó (entre 1 y 10)
int numeroSecreto = 7; // El número que la compu "pensó"
int intentoDelUsuario = 0; // Aquí guardamos lo que el usuario escribe
int intentosRealizados = 0;

Console.WriteLine("¡Ey, parcero! Adivina el número que estoy pensando (del 1 al 10).");

while (intentoDelUsuario != numeroSecreto)
{
    Console.Write("Escribe tu número y presiona Enter: ");
    // Convertimos lo que el usuario escribe (que es texto) a un número entero
    intentoDelUsuario = Convert.ToInt32(Console.ReadLine());
    intentosRealizados++; // Sumamos un intento

    if (intentoDelUsuario != numeroSecreto)
    {
        Console.WriteLine("¡Ush, no es ese! Sigue intentando, ¡vos podés!");
        if (intentoDelUsuario < numeroSecreto) {
            Console.WriteLine("(Una pista: el número secreto es más grande...)");
        } else {
            Console.WriteLine("(Una pista: el número secreto es más pequeño...)");
        }
    }
}

// Si el código llega aquí, es porque el while terminó, o sea, ¡adivinó!
Console.WriteLine("¡Esooo! ¡Adivinaste, máquina! El número era " + numeroSecreto + ".");
Console.WriteLine("Lo lograste en " + intentosRealizados + " intentos. ¡Sos un duro!");
```

**⚠️ ¡Cuidado con el "Guayabo Eterno" de los Ciclos! (Ciclos Infinitos)**

Con el ciclo `while`, hay que tener cuidado. Si la condición para que se detenga NUNCA se cumple, ¡el ciclo se queda repitiendo para siempre! A esto se le llama un **ciclo infinito**. Es como si el bus de Belén nunca llegara a su destino porque la condición para parar (llegar al paradero) nunca se da. ¡El programa se queda "pegado"!

```csharp
// ¡NUNCA HAGAN ESTO! EJEMPLO DE CICLO INFINITO:
// int tengoHambre = 1; // 1 significa que sí tengo hambre
// while (tengoHambre == 1)
// {
//     Console.WriteLine("Comiendo bandeja paisa...");
//     // ¡OJO! Aquí nunca cambio el valor de tengoHambre a 0 (ya no tengo hambre)
//     // ¡Así que esto se repetiría sin fin!
// }
```
Siempre asegúrense de que dentro del `while` haya algo que, en algún momento, haga que la condición se vuelva falsa para que el ciclo pueda terminar.

---

## 🧺 ¿Qué Son los Arreglos? - Tu Colección de Tazos, Pero en el Computador

¡Listo! Ya sabemos cómo hacer que el computador repita tareas. Ahora, ¿cómo guardamos un montón de datos juntos? Por ejemplo, la lista de sus amigos, las canciones de su playlist, o los ingredientes para el sancocho.

Para eso están los **Arreglos** (en inglés, "Arrays"). Un arreglo es como una cajita con varios compartimentos, donde cada compartimento guarda un dato. ¡Pero ojo! Usualmente, todos los datos en un arreglo son del mismo tipo (todos números, o todas palabras, etc.).

**Piénsenlo así:**

*   Una **lista de convocados** para el partido del Nacional o del Medellín. Todos son nombres de jugadores.
*   Su **playlist de Spotify** con sus canciones favoritas. Todas son títulos de canciones.
*   Una **cartuchera** donde guardan lapiceros de varios colores. Cada lapicero es un color.
*   Los **ingredientes** para una arepa: harina, agua, sal, quesito...

**Lo clave de los arreglos:**

1.  **Ordenados:** Cada elemento tiene una posición fija.
2.  **Índices:** Para saber dónde está cada elemento, usamos un **índice** (como un número de casillero). **¡MUY IMPORTANTE!** En C# (y muchos lenguajes), los índices empiezan a contar desde **CERO (0)**. Sí, ¡el primer elemento está en la posición 0, el segundo en la 1, y así! Es como si el primer piso de un edificio fuera el "piso 0".

**¿Cómo creamos y usamos arreglos en C#?**

```csharp
// Vamos a crear una lista (arreglo) de algunos parches pa' hacer en Medallo
string[] parchesEnMedellin = {"Ir al Parque Lleras", "Subir al Pueblito Paisa", "Caminar por la 70", "Visitar Guatapé (ok, es cerquita)", "Comer en el Mercado del Río"};

// ¿Cómo vemos el primer parche? (Recordemos: posición 0)
Console.WriteLine("El primer parche de mi lista es: " + parchesEnMedellin[0]); // Muestra "Ir al Parque Lleras"

// ¿Y el tercer parche? (Sería la posición 2)
Console.WriteLine("El tercer parche es: " + parchesEnMedellin[2]); // Muestra "Caminar por la 70"

// ¿Cuántos parches tengo en total? Usamos .Length (longitud)
Console.WriteLine("Tengo " + parchesEnMedellin.Length + " parches planeados. ¡Qué belleza!");

// ¿Qué pasa si intento ver un parche que no existe, por ejemplo, en la posición 10?
// Console.WriteLine(parchesEnMedellin[10]); // ¡Esto daría un error! Hay que tener cuidado.

// También podemos cambiar un elemento
parchesEnMedellin[0] = "Ir a una ciclovía nocturna"; // Cambiamos el primer parche
Console.WriteLine("Ahora el primer parche es: " + parchesEnMedellin[0]);
```

---

## 🤝 Ciclos y Arreglos Juntos: La Combinación Ganadora, ¡Como la Bandeja Paisa!

Ahora viene lo más chimba: ¡usar ciclos para recorrer los arreglos! Si tienen una lista de 100 amigos en un arreglo, ¿van a escribir 100 líneas de código para saludarlos uno por uno? ¡Ni locos! Usamos un ciclo.

**Ejemplo: Mostrar todos los parches de nuestra lista con un ciclo `for`:**

```csharp
string[] parchesEnMedellin = {"Ir a una ciclovía nocturna", "Subir al Pueblito Paisa", "Caminar por la 70", "Visitar Guatapé", "Comer en el Mercado del Río"};

Console.WriteLine("
--- ¡Mis Parches Favoritos en Medellín! ---");
// Usamos parchesEnMedellin.Length para que el ciclo sepa hasta dónde ir, sin importar cuántos parches haya.
for (int i = 0; i < parchesEnMedellin.Length; i++)
{
    // i va tomando los valores: 0, 1, 2, 3, 4
    Console.WriteLine("Parche #" + (i + 1) + ": " + parchesEnMedellin[i]);
}
```

**Resultado:**
```
--- ¡Mis Parches Favoritos en Medellín! ---
Parche #1: Ir a una ciclovía nocturna
Parche #2: Subir al Pueblito Paisa
Parche #3: Caminar por la 70
Parche #4: Visitar Guatapé
Parche #5: Comer en el Mercado del Río
```

**Una forma más "elegante" y breve de recorrer arreglos: el ciclo `foreach`**

El ciclo `foreach` es como decir: "Para cada elemento DENTRO de este arreglo, haz esto". Es súper útil cuando solo quieren recorrer el arreglo y usar cada elemento, sin preocuparse tanto por los índices.

```csharp
string[] comidasTipicasDeAntioquia = {"Bandeja Paisa", "Mondongo", "Sancocho Antioqueño", "Arepa con todo", "Mazamorra"};

Console.WriteLine("
--- ¡Antojos Paisas que Podemos Programar! ---");
foreach (string cadaComida in comidasTipicasDeAntioquia) // "cadaComida" es una variable temporal que toma el valor de cada elemento
{
    Console.WriteLine("¡Qué rico sería comer: " + cadaComida + "!");
}
```
Este `foreach` hace lo mismo que el `for` de arriba para mostrar los elementos, ¡pero con menos complique!

---

## 🛠️ ¡A "Echar Código"! Ejercicios Bien Paisas

¡Llegó la hora de practicar, parceros! Intenten resolver estos ejercicios en C#.

1.  **Lista de Tareas del Finde:**
    *   Crea un arreglo llamado `tareasDelFinde` con 5 tareas que suelan hacer un fin de semana en Medellín (ej: "Ir a la ciclovía", "Hacer tareas del colegio", "Visitar a la abuela", "Jugar fútbol en la cancha del barrio", "Salir con los parceros").
    *   Usa un ciclo `for` para imprimir cada tarea diciendo: "Este finde tengo que: [nombre de la tarea]".

2.  **Ahorrando pa' las Boletas:**
    *   Imagina que quieres ahorrar para las boletas de un concierto de tu artista favorito, que valen $150.000.
    *   Empiezas con $0 ahorrados.
    *   Cada "semana" (cada repetición del ciclo) ahorras $20.000 que te dan tus papás o que ganas haciendo "vuelticas".
    *   Usa un ciclo `while` para simular cuántas semanas necesitas ahorrar hasta que tengas suficiente para las boletas.
    *   Dentro del ciclo, muestra cuánto llevas ahorrado cada semana. Al final, di: "¡Listo! Ya tengo pa' las boletas después de X semanas."

3.  **Ídolos del Fútbol Paisa:**
    *   Crea un arreglo llamado `idolosDelFutbol` con 3 de tus jugadores favoritos (o históricos) del Nacional o del Medellín.
    *   Usa un ciclo `foreach` para imprimir el nombre de cada jugador con un mensaje bien emotivo, como: "¡Grande, [nombre del jugador], sos un crack!".

4.  **Ingredientes pa' la Arepa:**
    *   Crea un arreglo llamado `ingredientesArepa` con los ingredientes básicos para hacer una arepa paisa (ej: "Harina de maíz", "Agua tibia", "Sal", "Quesito").
    *   Usa un ciclo `for` o `foreach` para mostrar cada ingrediente.

5.  **Desafío: La Tiendita de la Esquina (¡Más Avanzado!)**
    *   Crea dos arreglos:
        *   productosTienda (string):
                "Gaseosa", "Papitas", "Chocolatina", "Buñuelo"
        *   preciosTienda (int): 
                2500, 1800, 1200, 1500 (Asegúrate que el orden corresponda con los productos).
    *   Simula una compra. Pregunta al usuario qué producto quiere comprar (puede ser por número, ej: 1 para Gaseosa, 2 para Papitas...).
    *   Usa un ciclo `while` para permitir que el usuario agregue varios productos a su "canasta" (puede ser una variable que sume el total).
    *   El ciclo debe terminar cuando el usuario decida no comprar más (puedes preguntarle "¿Desea agregar otro producto? S/N").
    *   Al final, muestra el total de la compra.
    *   **Pista:** Necesitarás leer la entrada del usuario (`Console.ReadLine()`) y convertirla a número si es necesario (`Convert.ToInt32()`).

---

## 📝 Pa' que no se te Olvide, Parse - Resumen y Consejos

*   **Ciclos `for`:** Cuando sabés cuántas veces. (Inicio, condición, incremento).
*   **Ciclos `while`:** Mientras una condición sea verdad. (¡Cuidado con los infinitos!).
*   **Arreglos (Arrays):** Cajitas para guardar listas de datos del mismo tipo. ¡Los índices empiezan en 0!
*   **`foreach`:** Forma fácil de recorrer todos los elementos de un arreglo.

**Consejos de un Parcero Programador:**

1.  **¡Practicá, practicá, practicá!** "Echar código" es la única forma de volverse un teso.
2.  **No te dé pena preguntar.** Si te enredás, ¡preguntá! A tus profes, a tus compañeros, en internet.
3.  **Usá `Console.WriteLine()` como tu mejor amigo.** Pa' ver qué está pasando en tu código, qué valores tienen las variables, etc. Es como ponerle "chismosos" a tu programa.
4.  **Leé código de otros.** Cuando veas ejemplos, trata de entender cómo funcionan.
5.  **¡Conectate con la comunidad!** En Medellín hay gente muy pila en esto:
    *   **MedellinJS** (Aunque es de JavaScript, se aprende mucho de lógica de programación)
    *   **.NET Medellín** (¡Perfecto para los que le están dando al C#!)
    *   **Ruta N** (Siempre tienen eventos ycharlas bacanas de tecnología)

---

## 🎉 ¡A Programar se Dijo, Pues!

¡Listo, futuro crack de la programación! Ya tenés las bases de los ciclos y arreglos. Ahora te toca a vos experimentar, crear cosas chéveres y, sobre todo, ¡divertirte aprendiendo!

Si tenés preguntas o querés mostrar lo que hiciste, ¡no dudes en compartirlo!

**¡Éxitos en tu camino como programador/a paisa!** 🇨🇴👨‍💻👩‍💻
