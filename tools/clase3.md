# Curso "¡Pura Magia Web con JavaScript!" ✨🧙‍♂️
## Dale Vida, Inteligencia y ¡Bacaneo! a tus Páginas Web

**Para:** Jóvenes bacanos y bacanas de 15 a 17 años de Medellín, Antioquia (¡los que ya saben HTML, CSS y entienden el mundo web!).
**Duración Estimada:** Unas 4 horas de parche, lógica y ¡mucha interacción!
**Nivel:** Introductorio a JavaScript (¡el lenguaje que le da el toque!).

---

### **📝 Nota Importante para Navegar este Archivo:**

Este documento es tu libro de hechizos para darle vida a tus páginas.
*   **Lee con calma:** JavaScript es un lenguaje de programación real. Tómate tu tiempo para entender cada concepto.
*   **Haz las actividades en tu computador:** ¡Es CLAVE! Escribir, ejecutar y ver los resultados es la mejor forma de aprender.
*   **No te asustes con los errores:** Los errores son tus amigos en programación. Te dicen dónde te equivocaste para que aprendas. ¡Todos los programadores cometen errores!
*   **¡Experimenta!** Cambia valores, prueba lógica diferente. ¡Así es como se aprende de verdad!
*   **¡Pregunta!** Si estás en un grupo, discutan las dudas. Si estás solo, anota tus preguntas.
*   **¡Diviértete!** Ver cómo tu página reacciona a tus instrucciones es una sensación muy chimba.

---

## 🎯 **Objetivos de este Parche "Mago Web":**

Al final de este curso, vas a ser un "teso" (o "tesa") en el JavaScript básico, capaz de:
*   Entender qué es **JavaScript**, para qué sirve y cómo se conecta con HTML y CSS.
*   Conocer los **tipos de datos básicos** que usa JavaScript.
*   Manejar **variables** para guardar información.
*   Entender los **operadores** para hacer cálculos y comparaciones.
*   Usar las **estructuras de control (condicionales)** para que tu código tome decisiones.
*   Crear tus primeras **funciones** para reutilizar código.
*   Interactuar con tu página web usando el **DOM** (Document Object Model).
*   Responder a **eventos** (clics de usuario, movimientos del mouse).

---

## 📚 **¿Qué Necesitas para este Parche de Programación?**

*   Tu computador con **VS Code** instalado.
*   Un navegador web (Chrome, Firefox, Edge, Safari).
*   Los archivos de tu proyecto anterior (ej. `mi-primera-pagina.html` y `estilos.css`).
*   Mucha paciencia y ganas de "echar código".

---

## ⏰ **¡A Ponerle Ambiente a la Clase! (Organización por Bloques)**

---

### **Bloque 1: JavaScript - ¡El Cerebro de tu Página! (Aprox. 1 hora)**

*   #### **1.1. Bienvenida y ¿Qué es JavaScript? (15 min)**
    *   **Recordando:** Ya sabemos que HTML es el esqueleto, CSS es la ropa y el maquillaje. ¿Pero cómo hacemos que nuestra página se mueva, reaccione, haga cosas? ¡Ahí entra JavaScript!
    *   **¿Qué es JavaScript?**
        *   Es un **lenguaje de programación** (¡este sí es un lenguaje de programación de verdad!).
        *   Es el **cerebro** de la web. Le da interactividad y dinamismo a tus páginas.
        *   Corre principalmente en el **navegador del cliente** (Frontend).
        *   Permite que la página **haga cosas**: validar formularios, animaciones, juegos, mostrar mensajes, cambiar contenido, etc.
    *   **Analogías:**
        *   Si la web es un carro: HTML es el chasis, CSS es la pintura y los accesorios, **JavaScript es el motor, la dirección y la electrónica** que lo hacen funcionar.
        *   Si la web es un cuerpo: HTML es el esqueleto, CSS es la piel y la ropa, **JavaScript son los músculos y el cerebro** que permiten que se mueva y piense.

*   #### **1.2. Tu Primer "Hola Mundo" en JavaScript (20 min)**
    *   **Conectando JS con HTML:**
        1.  **Crea un nuevo archivo JavaScript:** En VS Code, crea `script.js` en la *misma carpeta* que tu `mi-primera-pagina.html`.
        2.  **Linkea JS en HTML:** Abre `mi-primera-pagina.html`. Justo **antes de la etiqueta de cierre `</body>`**, agrega esta línea:
            ```html
            <script src="script.js"></script>
            ```
            *   **¡Importante!** La etiqueta `<script>` suele ir al final del `<body>` para que el HTML y CSS se carguen primero y JavaScript pueda interactuar con ellos sin problemas.
            *   *Guarda `mi-primera-pagina.html`.*
    *   **Tu Primer Comando:**
        1.  **Abre `script.js`** y escribe:
            ```javascript
            alert("¡Hola, Medellín! Mi primera alerta con JS.");
            console.log("¡Este mensaje lo veo en la consola!");
            ```
        2.  **Guarda `script.js`.**
        3.  **Abre `mi-primera-pagina.html` en tu navegador.**
            *   Deberías ver una ventana emergente (un "alert") con tu mensaje.
            *   Después de cerrar la alerta, haz clic derecho -> "Inspeccionar" -> Pestaña "Console" (Consola). ¡Ahí verás el mensaje de `console.log`!
            *   `alert()`: Muestra un mensaje al usuario en una ventana emergente.
            *   `console.log()`: Muestra mensajes en la consola del navegador, ¡súper útil para depurar y ver qué está pasando por dentro!

*   #### **1.3. Datos y Variables: ¡Guardando Información! (25 min)**
    *   **¿Qué son los Datos?** Son la información con la que trabaja JavaScript (ej. tu nombre, tu edad, si te gusta el fútbol).
    *   **Tipos de Datos Comunes:**
        *   **Strings (Cadenas de Texto):** Texto, siempre entre comillas. (Ej: `"Juan"`, `"Medellín"`, `"Hola"`)
        *   **Numbers (Números):** Números enteros o decimales. (Ej: `18`, `3.14`, `1000`)
        *   **Booleans (Booleanos):** Verdadero o falso. (Ej: `true`, `false`)
        *   **Arrays (Arreglos/Listas):** Una lista de cosas. (Ej: `["fútbol", "música", "videojuegos"]`)
        *   **Objects (Objetos):** Representan cosas con propiedades. (Ej: `{ nombre: "Pedro", edad: 17 }`)
    *   **¿Qué son las Variables?** Son como "cajas" con un nombre donde guardamos datos. El contenido de la caja puede cambiar.
        *   Se declaran con `let` o `const`.
            *   `let`: La "caja" puede cambiar su contenido. (Ej: `let edad = 17; edad = 18;`)
            *   `const`: La "caja" tiene un contenido que NO puede cambiar. (Ej: `const PI = 3.1416;`)
    *   **Actividad: ¡Crea tus primeras variables!**
        *   En `script.js`, borra lo anterior (o déjalo comentado con `//` para una línea o `/* ... */` para varias) y escribe:
            ```javascript
            // Variables para mi información
            let miNombre = "Tu Nombre"; // Un String
            let miEdad = 17; // Un Number
            const ciudadNacimiento = "Medellín"; // Un String (no cambia)
            let meGustaProgramar = true; // Un Boolean

            // Un Array de hobbies
            let misHobbies = ["Jugar Free Fire", "Escuchar Reggaetón", "Montar en bici"];

            // Un Objeto para representar a un amigo
            let amigo = {
                nombre: "Carlos",
                edad: 16,
                ciudad: "Envigado"
            };

            console.log("Mi nombre es: " + miNombre); // Unimos texto con una variable
            console.log("Tengo " + miEdad + " años.");
            console.log("¿Me gusta programar? " + meGustaProgramar);
            console.log("Mi primer hobby es: " + misHobbies[0]); // El [0] es para acceder al primer elemento del arreglo
            console.log("El nombre de mi amigo es: " + amigo.nombre); // Accedemos a una propiedad del objeto

            // Cambiando una variable (solo con let)
            miEdad = 18;
            console.log("¡Ahora tengo " + miEdad + " años!");
            ```
            *Guarda `script.js` y mira la consola en el navegador.*

---

### **Bloque 2: Operadores y Decisiones: ¡JavaScript Piensa! (Aprox. 1 hora)**

*   #### **2.1. Operadores: ¡Calculando y Comparando! (25 min)**
    *   Los operadores son símbolos que nos permiten hacer operaciones con los datos.
    *   **Operadores Aritméticos (¡para calcular!):**
        *   `+` (Suma)
        *   `-` (Resta)
        *   `*` (Multiplicación)
        *   `/` (División)
        *   `%` (Módulo - el residuo de una división)
    *   **Operadores de Comparación (¡para preguntar!):** Siempre devuelven un `boolean` (`true` o `false`).
        *   `==` (Igual a - compara el valor, no el tipo)
        *   `===` (Estrictamente igual a - compara valor Y tipo, ¡es el recomendado!)
        *   `!=` (Diferente de - compara el valor)
        *   `!==` (Estrictamente diferente de - compara valor Y tipo, ¡el recomendado!)
        *   `>` (Mayor que)
        *   `<` (Menor que)
        *   `>=` (Mayor o igual que)
        *   `<=` (Menor o igual que)
    *   **Operadores Lógicos (¡para conectar preguntas!):**
        *   `&&` (AND - "y"): `true` si AMBAS condiciones son `true`.
        *   `||` (OR - "o"): `true` si UNA de las condiciones es `true`.
        *   `!` (NOT - "no"): Invierte el valor (`true` se vuelve `false`, `false` se vuelve `true`).
    *   **Actividad: ¡Calculando el descuento!**
        *   En `script.js`:
            ```javascript
            let precioProducto = 50000; // 50 mil pesos
            let descuento = 0.10; // 10% de descuento

            let precioFinal = precioProducto - (precioProducto * descuento);
            console.log("Precio original: " + precioProducto + " pesos.");
            console.log("Descuento aplicado: " + (descuento * 100) + "%");
            console.log("Precio con descuento: " + precioFinal + " pesos.");

            let tieneTarjetaClub = true;
            let esFinDeSemana = false;

            // Comparaciones
            console.log("¿El precio final es menor que 45000? " + (precioFinal < 45000));
            console.log("¿Tiene tarjeta Y es fin de semana? " + (tieneTarjetaClub && esFinDeSemana));
            console.log("¿Tiene tarjeta O es fin de semana? " + (tieneTarjetaClub || esFinDeSemana));
            ```
            *Guarda y mira la consola.*

*   #### **2.2. Condicionales `if-else`: ¡JavaScript toma Decisiones! (25 min)**
    *   Las condicionales permiten que tu código haga una cosa o la otra, dependiendo de si una condición es verdadera (`true`) o falsa (`false`).
    *   **Sintaxis `if`:**
        ```javascript
        if (condicion_es_verdadera) {
            // Haz esto
        }
        ```
    *   **Sintaxis `if-else`:**
        ```javascript
        if (condicion_es_verdadera) {
            // Haz esto
        } else {
            // Si no, haz esto otro
        }
        ```
    *   **Sintaxis `if-else if-else` (varias opciones):**
        ```javascript
        if (condicion1) {
            // Si se cumple la condición 1
        } else if (condicion2) {
            // Si no, y se cumple la condición 2
        } else {
            // Si no se cumple ninguna de las anteriores
        }
        ```
    *   **Actividad: ¡Decide si puedes entrar a la fiesta!**
        *   En `script.js`:
            ```javascript
            let tuEdad = 17;
            const edadMinimaFiesta = 18;
            let tienesInvitacion = true;

            if (tuEdad >= edadMinimaFiesta && tienesInvitacion) {
                console.log("¡Bienvenido a la fiesta, parce! Disfruta la rumba.");
            } else if (tuEdad >= edadMinimaFiesta && !tienesInvitacion) {
                console.log("Podes pasar, pero la próxima vez trae invitación.");
            }
            else {
                console.log("Lo siento, parcero. Eres menor de edad o no tienes invitación. ¡Nos vemos en la próxima!");
            }

            // Otro ejemplo: ¿Qué hora es?
            let horaActual = new Date().getHours(); // Obtiene la hora actual del sistema (0-23)

            if (horaActual < 12) {
                console.log("¡Buenos días!");
            } else if (horaActual < 19) {
                console.log("¡Buenas tardes!");
            } else {
                console.log("¡Buenas noches!");
            }
            ```
            *Guarda y mira la consola.* ¡Juega con el valor de `tuEdad` y `tienesInvitacion` para ver los diferentes resultados!

*   #### **2.3. Funciones: ¡Recetas Reutilizables de Código! (10 min)**
    *   Una función es un bloque de código que realiza una tarea específica y que puedes **llamar y reutilizar** cuando la necesites. ¡Es como una receta de cocina!
    *   **Sintaxis:**
        ```javascript
        function nombreDeLaFuncion(parametro1, parametro2) {
            // Código que se ejecuta cuando llamas a la función
            // Puedes usar los parámetros aquí
            return algo; // Opcional: la función puede devolver un valor
        }
        ```
    *   **Actividad: ¡Crea tu propia función de saludo!**
        *   En `script.js`:
            ```javascript
            function saludar(nombre) {
                console.log("¡Hola, " + nombre + "! ¿Cómo va todo?");
            }

            // Llamar a la función
            saludar("Juan");
            saludar("Ana");
            saludar(miNombre); // Usamos nuestra variable del Bloque 1
            ```
            *Guarda y mira la consola.*

---

### **Bloque 3: DOM y Eventos - ¡Interactuando con la Página! (Aprox. 1 hora)**

*   #### **3.1. El DOM: ¡El Mapa de tu Página! (25 min)**
    *   **DOM (Document Object Model):** ¡Es la clave de la interactividad! Piensen que el navegador, cuando carga su HTML, crea un "mapa" o un "árbol" de todos los elementos de la página. Este mapa se llama DOM.
    *   JavaScript puede "navegar" por este mapa, **encontrar elementos HTML** (títulos, párrafos, imágenes, botones) y **cambiar su contenido, su estilo o sus atributos.**
    *   **Cómo encontrar elementos (¡los más comunes!):**
        *   `document.getElementById("id-del-elemento")`: Busca un elemento por su `id`. (¡Recuerdan el `id` en HTML?).
        *   `document.querySelector(".clase-del-elemento")`: Busca el primer elemento que tenga esa `class` o etiqueta.
        *   `document.querySelectorAll(".clase-del-elemento")`: Busca *todos* los elementos que tengan esa `class`.
    *   **Cómo cambiar elementos:**
        *   `.textContent = "Nuevo texto";`: Cambia el texto dentro del elemento.
        *   `.innerHTML = "<b>Nuevo</b> contenido HTML";`: Cambia el contenido, ¡puedes poner hasta HTML dentro!
        *   `.style.backgroundColor = "blue";`: Cambia un estilo CSS directamente.
        *   `.classList.add("nombre-clase");`: Agrega una clase CSS (¡lo mejor!).
        *   `.classList.remove("nombre-clase");`: Quita una clase CSS.
    *   **Actividad: ¡Cambia el título y un párrafo!**
        1.  **En `mi-primera-pagina.html`**, vamos a darle un `id` a nuestro `h1` y a un párrafo:
            ```html
            <header>
                <h1 id="titulo-principal">¡Hola, Parceros! Soy [Tu Nombre]</h1>
                <!-- ... resto del header ... -->
            </header>

            <main>
                <section id="sobre-mi">
                    <h2>Sobre Mí:</h2>
                    <p id="parrafo-principal">Nací en [Tu Barrio o Ciudad] y vivo en [Tu Barrio o Ciudad]. Me gusta mucho <span class="destacado">tu Hobby o Deporte favorito</span>.</p>
                    <!-- ... resto de la sección ... -->
                </section>
            </main>
            ```
            *Guarda `mi-primera-pagina.html`.*
        2.  **En `script.js`**, agrega:
            ```javascript
            // 1. Encontrar el título principal por su ID
            let titulo = document.getElementById("titulo-principal");

            // 2. Cambiar su texto
            titulo.textContent = "¡Mi Página Bacana con JavaScript!";

            // 3. Encontrar el párrafo principal
            let parrafo = document.getElementById("parrafo-principal");

            // 4. Cambiar su contenido HTML (agregando un emoji)
            parrafo.innerHTML = "¡Esta página ahora es <b>interactiva</b> con JavaScript! 🚀";

            // 5. Cambiar el estilo directamente (no es lo más recomendado, pero se puede)
            parrafo.style.color = "purple";
            parrafo.style.fontWeight = "bold";
            ```
            *Guarda `script.js` y actualiza tu página.* ¡Verás cómo JavaScript cambió lo que tenías en el HTML!

*   #### **3.2. Eventos: ¡Cuando el Usuario Hace Algo! (25 min)**
    *   Los eventos son cosas que pasan en la página (el usuario hace clic en un botón, pasa el mouse por una imagen, escribe en un campo, la página termina de cargar).
    *   JavaScript nos permite "escuchar" esos eventos y **responder** a ellos con código.
    *   **`addEventListener()`:** Es la forma más común y recomendada para escuchar eventos.
        ```javascript
        elemento.addEventListener("tipoDeEvento", funcionAEjecutar);
        ```
        *   `elemento`: El elemento HTML al que le vas a "escuchar" el evento (ej. un botón).
        *   `"tipoDeEvento"`: El nombre del evento (ej. `"click"`, `"mouseover"`, `"submit"`).
        *   `funcionAEjecutar`: La función que se activará cuando el evento ocurra.
    *   **Actividad: ¡Un botón para saludar!**
        1.  **En `mi-primera-pagina.html`**, agrega un botón debajo de tu `section id="sobre-mi"`:
            ```html
            <button id="boton-saludar">¡Salúdame!</button>
            ```
            *Guarda `mi-primera-pagina.html`.*
        2.  **En `script.js`**, agrega:
            ```javascript
            // 1. Encontrar el botón
            let botonSaludar = document.getElementById("boton-saludar");

            // 2. Definir la función que se ejecutará cuando hagan clic
            function alHacerClick() {
                alert("¡Qué más, parcero! Te saluda tu página web.");
                console.log("Se hizo clic en el botón.");

                // Podemos cambiar el texto del botón después de hacer clic
                botonSaludar.textContent = "¡Ya te saludé!";
                botonSaludar.style.backgroundColor = "lightgreen";
            }

            // 3. "Escuchar" el evento click en el botón y llamar a la función
            botonSaludar.addEventListener("click", alHacerClick);
            ```
            *Guarda `script.js` y actualiza tu página.* **¡Haz clic en el botón y mira la magia!**

*   #### **3.3. Taller: ¡Un Contador de "Likes" Sencillo! (10 min)**
    *   **Actividad:** Vamos a crear un contador de "likes" como los de redes sociales.
        1.  **En `mi-primera-pagina.html`**, agrega un nuevo `div` con un botón de "Like" y un párrafo para mostrar el conteo:
            ```html
            <section style="text-align: center; margin-top: 40px;">
                <h3>¡Dale Like!</h3>
                <p>Likes: <span id="contador-likes">0</span></p>
                <button id="boton-like">👍 Like</button>
            </section>
            ```
            *Guarda `mi-primera-pagina.html`.*
        2.  **En `script.js`**, agrega:
            ```javascript
            let contador = 0; // Variable para guardar los likes
            let elementoContador = document.getElementById("contador-likes");
            let botonLike = document.getElementById("boton-like");

            function agregarLike() {
                contador = contador + 1; // Sumamos 1 al contador
                elementoContador.textContent = contador; // Actualizamos el texto en la página
                console.log("Nuevo like! Total: " + contador);

                // Si llega a 5 likes, cambiamos el color del botón
                if (contador === 5) {
                    botonLike.style.backgroundColor = "#2ecc71"; // Verde
                    botonLike.textContent = "¡Gracias por los Likes! 🎉";
                }
            }

            botonLike.addEventListener("click", agregarLike);
            ```
            *Guarda `script.js` y actualiza tu página.* **¡Haz clic varias veces en el botón "Like" y mira cómo se actualiza el contador y cambia el botón!**

---

### **Bloque 4: Cierre y ¡A Seguir Codificando! (Aprox. 1 hora)**

*   #### **4.1. Repaso Rápido: ¡La Magia que Aprendimos! (15 min)**
    *   **Preguntas y Respuestas (abiertas):**
        *   ¿Para qué sirve JavaScript en una página web?
        *   Nombra 3 tipos de datos en JS.
        *   ¿Cuál es la diferencia entre `let` y `const`?
        *   ¿Para qué sirve un `if-else`?
        *   ¿Qué es el DOM y por qué es importante?
        *   ¿Qué es un evento y cómo lo "escuchamos"?
    *   **Recapitulando:** Hoy dimos un salto gigante. Pasamos de páginas estáticas a páginas que piensan, reaccionan y hacen cosas gracias a JavaScript. Aprendimos a guardar información, tomar decisiones, crear funciones reutilizables y, lo más emocionante, ¡interactuar con nuestra página y responder a lo que el usuario hace!

*   #### **4.2. Mini-Evaluación o Desafío de Interacción (30 min)**
    *   **Actividad Individual o en Parejas: "¡Mi Mini-App Interactiva!"**
        *   **En tu `mi-primera-pagina.html` (o crea un nuevo archivo):**
            *   Agrega un párrafo con un ID (ej. `<p id="mensaje-bienvenida">Haz clic en el botón</p>`).
            *   Agrega un botón con un ID (ej. `<button id="cambiar-saludo">Cambiar Saludo</button>`).
            *   Agrega una imagen con un ID (ej. `<img id="imagen-cambiante" src="[URL_IMAGEN_1]">`).
        *   **En tu `script.js`:**
            *   Crea una variable para guardar un estado (ej. `let saludoActual = 1;`).
            *   Crea una función que, al hacer clic en el botón:
                *   Cambie el texto del párrafo (`mensaje-bienvenida`) por un nuevo saludo diferente cada vez que se haga clic.
                *   Si el `saludoActual` llega a un número (ej. 3), que cambie la imagen (`imagen-cambiante`) por otra URL diferente y cambie el color del botón.
                *   Usa `if-else` para las decisiones y `document.getElementById()` para encontrar los elementos.
        *   **Comparte (si estás en grupo):** Muestra cómo tu página interactúa y explica el código que usaste.

*   #### **4.3. Cierre y El Futuro: ¡El Límite es tu Imaginación! (15 min)**
    *   **Mensaje Final:** ¡Lo que aprendieron hoy es la base para crear todo tipo de aplicaciones web interactivas! Desde juegos simples hasta calculadoras, formularios dinámicos y hasta la interacción de una red social. ¡El JavaScript es el lenguaje más demandado en la web!
    *   **¿Y Ahora Qué Sigue?**
        *   **Más JavaScript:** Bucles (`for`, `while`), Arrays y Objetos más a fondo, manipulación de Strings.
        *   **APIs (Application Programming Interfaces):** Cómo JavaScript puede pedir información a otros servicios (ej. información del clima, fotos de Unsplash).
        *   **Asincronía:** Cómo hacer que tu página no se bloquee mientras espera datos del servidor.
        *   **Frameworks de JavaScript:** React, Vue, Angular. ¡Herramientas avanzadas que te permiten construir aplicaciones enormes y súper eficientes! (¡Ahí es donde se ponen las cosas súper bacanas!).

---

¡Felicitaciones, futuros magos del código! ¡Están a punto de darle vida a la web! ¡Sigan practicando y creando, que el mundo digital necesita su talento!