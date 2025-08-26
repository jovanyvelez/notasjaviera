# Curso "¡Pura Pinta Web - Nivel 2!" 🚀✨
## Estructura con Sentido, Diseño Inteligente y ¡Listos para el Celular!

**Para:** Jóvenes bacanos y bacanas de 15 a 17 años de Medellín, Antioquia (¡los mismos que ya saben lo básico de HTML y CSS!).
**Duración Estimada:** Unas 4 horas de parche y código (¡pero a tu ritmo!).
**Nivel:** Intermedio Básico (¡construyendo sobre lo que ya sabes!).

---

### **📝 Nota Importante para Navegar este Archivo:**

Este documento es la continuación de tu aventura web.
*   **Recuerda lo básico:** Ten a mano lo que aprendiste de HTML y CSS. ¡Lo vamos a usar mucho!
*   **Haz las actividades en tu computador:** Es la única forma de que se te quede grabado y veas los resultados de inmediato.
*   **No tengas miedo a experimentar:** Cambia colores, tamaños, posiciones. ¡Así es como se descubren cosas nuevas!
*   **¡Pregunta!** Si estás en un grupo, discutan las dudas. Si estás solo, anota tus preguntas.
*   **¡Diviértete!** Ver cómo tu página se transforma y se adapta es muy gratificante.

---

## 🎯 **Objetivos de este Nuevo Parche Web:**

Al final de este curso, vas a ser un "teso" (o "tesa") en la web intermedia, capaz de:
*   Usar etiquetas HTML que le den más **sentido y estructura** a tu página (¡HTML semántico!).
*   Manejar **fuentes de Google Fonts** para que tu texto tenga una pinta más pro.
*   Aplicar **sombras** a tus textos y cajas para que se vean más estéticas.
*   Dominar los fundamentos de **Flexbox** para organizar tus elementos en línea y columnas de forma fácil.
*   Hacer tu página **"responsive"** (adaptable) para que se vea bien en celulares, tablets y computadores grandes (¡con las famosas **Media Queries**!).

---

## 📚 **¿Qué Necesitas para este Parche de Programación?**

*   Tu computador con **VS Code** instalado.
*   Un navegador web (Chrome, Firefox, Edge, Safari).
*   Los archivos `mi-primera-pagina.html` y `estilos.css` que creaste en el curso anterior (¡o crea unos nuevos!).
*   Ganas de seguir aprendiendo y creando.

---

## ⏰ **¡A Ponerle Ambiente a la Clase! (Organización por Bloques)**

---

### **Bloque 1: HTML Semántico - ¡Tu Esqueleto con Sentido! (Aprox. 1 hora)**

*   #### **1.1. ¡Recordemos el Esqueleto! (10 min)**
    *   **Discusión/Reflexión:** ¿Recuerdan que en el curso anterior usábamos mucho el `<div>` para agrupar contenido? Era como una "caja genérica".
    *   **El problema del `<div>` excesivo:** Es como si una casa solo tuviera paredes sin saber dónde está la cocina, dónde la sala. El navegador (y otros programas) no saben qué es importante y qué no.
    *   **La solución: HTML Semántico.** Son etiquetas que le dan un significado a las secciones de tu página.

*   #### **1.2. Etiquetas con Significado: ¡Dale Orden a tu Contenido! (35 min)**
    *   Estas etiquetas son como darle un nombre a cada habitación de tu casa. No cambian el aspecto visual, pero le dicen al navegador (y a Google) qué tipo de contenido hay ahí.
    *   **Pilas con estas etiquetas semánticas:**
        *   **`<header>`:** La cabecera de la página o de una sección. Aquí suelen ir el logo, el título principal, un menú.
        *   **`<nav>`:** Un contenedor para el menú de navegación (los enlaces principales).
        *   **`<main>`:** El contenido principal y único de tu página. ¡Solo debería haber un `<main>` por página!
        *   **`<section>`:** Una sección temática de la página. Puedes tener varias.
        *   **`<article>`:** Contenido independiente que podría tener sentido por sí solo (ej. una noticia, un post de blog, una publicación de redes).
        *   **`<aside>`:** Contenido que está relacionado con el contenido principal pero que podría ir aparte (ej. una barra lateral, anuncios, un recuadro de "artículos relacionados").
        *   **`<footer>`:** El pie de página de la página o de una sección. Aquí suele ir información de contacto, derechos de autor, enlaces secundarios.
    *   **Actividad: ¡Reestructurando `mi-primera-pagina.html`!**
        1.  **Abre tu archivo `mi-primera-pagina.html`** en VS Code.
        2.  Vamos a cambiar los `<div>` genéricos por etiquetas semánticas.
        3.  Modifica tu `<body>` para que se vea así:
            ```html
            <body>
                <header>
                    <h1>¡Hola, Parceros! Soy [Tu Nombre]</h1>
                    <nav>
                        <ul>
                            <li><a href="#sobre-mi">Sobre Mí</a></li>
                            <li><a href="#hobbies">Mis Hobbies</a></li>
                            <li><a href="#contacto">Contacto</a></li>
                        </ul>
                    </nav>
                </header>

                <main>
                    <section id="sobre-mi">
                        <h2>Sobre Mí:</h2>
                        <p>Nací en [Tu Barrio o Ciudad] y vivo en [Tu Barrio o Ciudad]. Me gusta mucho <span class="destacado">tu Hobby o Deporte favorito</span>.</p>
                        <!-- Aquí va la imagen que ya tenías -->
                        <img src="URL_DE_TU_IMAGEN_DE_INTERNET" alt="Vista aérea de Medellín">
                        <p>¡Aquí estoy yo! (o la imagen de tu lugar favorito de Medellín).</p>
                    </section>

                    <section id="hobbies">
                        <h3>Mis Hobbies:</h3>
                        <ol>
                            <li>[Tu Videojuego #1]</li>
                            <li>[Tu Videojuego #2]</li>
                            <li>[Tu Videojuego #3]</li>
                        </ol>
                        <h3>Mis Comidas Favoritas:</h3>
                        <ul>
                            <li>Bandeja Paisa</li>
                            <li>Arepa con Hogao</li>
                            <li>Empanadas (¡obvio!)</li>
                            <li>Salchipapa</li>
                        </ul>
                    </section>

                    <aside>
                        <h4>Un Dato Curioso:</h4>
                        <p>¿Sabías que Medellín tiene el Metro más chimba del mundo?</p>
                    </aside>
                </main>

                <footer id="contacto">
                    <p>Contáctame en mis redes sociales: [Aquí puedes poner enlaces a tus redes, si quieres]</p>
                    <p>&copy; 2024 [Tu Nombre]. Todos los derechos reservados.</p>
                    <p>Visita <a href="https://www.medellin.gov.co/" target="_blank">la página oficial de Medellín</a>.</p>
                </footer>

            </body>
            ```
        *   **Guarda el archivo y actualiza en tu navegador.** ¡Visualmente no cambió nada, pero tu página ahora es más "inteligente" para el navegador!

*   #### **1.3. ¿Por qué es importante el HTML Semántico? (15 min)**
    *   **Para el navegador:** Entiende mejor la estructura.
    *   **Para los buscadores (Google):** Ayuda a posicionar mejor tu página (¡SEO!). Si Google sabe que algo es un `<nav>`, entiende que es un menú.
    *   **Para la accesibilidad:** Las personas que usan lectores de pantalla (para personas con discapacidad visual) pueden navegar tu página de forma más eficiente.
    *   **Para otros desarrolladores (y para ti mismo en el futuro):** ¡El código es más fácil de leer y entender!

---

### **Bloque 2: CSS - ¡Letras con Pinta y Detalles Estéticos! (Aprox. 1 hora)**

*   #### **2.1. ¡Fuentes Personalizadas! Con Google Fonts (25 min)**
    *   Las fuentes (tipografías) predeterminadas del navegador a veces son aburridas. ¡Vamos a usar Google Fonts para darle más personalidad!
    *   **Pasos para usar Google Fonts:**
        1.  **Ve a Google Fonts:** Abre tu navegador y busca `Google Fonts`. Entra a la página.
        2.  **Elige una fuente que te guste:** Explora las opciones. Cuando encuentres una, haz clic en ella.
        3.  **Selecciona los estilos:** Verás diferentes "pesos" (delgadez/grosor) de la fuente (ej. Regular 400, Bold 700). Selecciona los que quieras (haz clic en `+ Select`).
        4.  **Copia el código `<link>`:** En el panel de la derecha, busca la sección "Use on the web" y copia el código que empieza con `<link rel="preconnect"...`.
        5.  **Pega el `<link>` en tu HTML:** Abre `mi-primera-pagina.html`. Pega ese código que copiaste **dentro de la etiqueta `<head>`**, justo *antes* de tu `link rel="stylesheet" href="estilos.css"`.
        6.  **Copia la propiedad CSS:** En el mismo panel de Google Fonts, busca "CSS rules to specify families" y copia el `font-family` (ej. `font-family: 'Roboto', sans-serif;`).
        7.  **Pega el `font-family` en tu CSS:** Abre `estilos.css`. Pega esa propiedad en el selector `body { ... }` para que aplique a toda tu página, o en selectores específicos si solo quieres que una sección tenga esa fuente.
    *   **Actividad: ¡Cambia la fuente de tu página!**
        *   Elige una fuente de Google Fonts (ej. `Poppins`, `Open Sans`, `Montserrat`).
        *   Sigue los pasos y aplícala a tu `body` en `estilos.css`.
        *   *Guarda los dos archivos y actualiza tu página.* ¡Verás cómo cambia toda la pinta!

*   #### **2.2. ¡Luces y Sombras! `text-shadow` y `box-shadow` (20 min)**
    *   Las sombras le dan profundidad y un toque más pro a tu diseño.
    *   **`text-shadow` (Sombra para texto):**
        *   `text-shadow: 2px 2px 4px gray;`
        *   **Valores:** `[desplazamiento-X] [desplazamiento-Y] [desenfoque] [color];`
    *   **`box-shadow` (Sombra para cajas/elementos):**
        *   `box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);`
        *   **Valores:** `[desplazamiento-X] [desplazamiento-Y] [desenfoque] [expansión opcional] [color];`
        *   `rgba(0, 0, 0, 0.2)` es un color negro con 20% de transparencia.
    *   **Actividad: ¡Agrega sombras a tu página!**
        *   Abre `estilos.css`.
        *   Agrega una sombra a tu título principal `h1`:
            ```css
            h1 {
                /* ... otros estilos que ya tenías ... */
                text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.3); /* Una sombra suave */
            }
            ```
        *   Agrega una sombra a tu `section-sobre-mi` o a la nueva `<section>` que creaste:
            ```css
            .seccion-sobre-mi { /* O si le pusiste un ID a tu section, usa #tu-id */
                /* ... otros estilos ... */
                box-shadow: 0 8px 16px rgba(0, 0, 0, 0.15); /* Una sombra más notoria */
            }
            ```
            *Guarda y actualiza.* ¡Mira cómo los elementos tienen más profundidad!

*   #### **2.3. Colores Avanzados: RGB y HSL (15 min)**
    *   Ya conoces los nombres de colores (red, blue) y los hexadecimales (`#FF0000`).
    *   **RGB (Red, Green, Blue):** `rgb(255, 0, 0)` es rojo. Cada número va de 0 a 255. `rgba(255, 0, 0, 0.5)` agrega un canal alfa para la transparencia (0 es totalmente transparente, 1 es totalmente opaco).
    *   **HSL (Hue, Saturation, Lightness):** `hsl(0, 100%, 50%)` es rojo. Es más intuitivo para elegir colores.
        *   **Hue (Tono):** Un ángulo en la rueda de colores (0-360).
        *   **Saturation (Saturación):** Qué tan puro o gris es el color (0-100%).
        *   **Lightness (Luminosidad):** Qué tan oscuro o claro es el color (0-100%).
    *   **Actividad: ¡Experimenta con RGB/HSL!**
        *   En tu `estilos.css`, busca un color que ya tengas (ej. `color: #333;`).
        *   Cámbialo a `rgb(51, 51, 51);` o `hsl(0, 0%, 20%);` (es el mismo gris oscuro).
        *   **¡Juega con la transparencia!** Cambia el `background-color` de una sección a `rgba(255, 255, 255, 0.8);` para que sea blanco semitransparente.
            *Guarda y actualiza.*

---

### **Bloque 3: CSS Flexbox - ¡Organizando el Parche! (Aprox. 1 hora)**

*   #### **3.1. ¿Cuál es el problema y cómo lo resuelve Flexbox? (15 min)**
    *   **El problema:** Antes, organizar elementos en una fila o columna, o centrarlos, era un dolor de cabeza en CSS. Había que hacer trucos complicados.
    *   **La solución: Flexbox (Flexible Box Layout).** ¡Es una herramienta mágica para alinear y distribuir elementos en una sola dimensión (fila o columna)! Es como tener un control remoto para organizar tus "cajas".
    *   **Concepto clave:** Necesitas un **contenedor "flex"** (el padre) y **elementos "flex"** (los hijos).

*   #### **3.2. Propiedades de Flexbox: ¡El Control Remoto! (30 min)**
    *   **En el contenedor (el padre):**
        *   `display: flex;`: ¡Activa Flexbox! Convierte a este elemento en un contenedor flexible.
        *   `flex-direction: row;` (por defecto, los pone en fila) o `column;` (los pone en columna).
        *   `justify-content:` Cómo se distribuyen los elementos a lo largo del **eje principal** (horizontal si es `row`, vertical si es `column`).
            *   `flex-start;` (al inicio)
            *   `flex-end;` (al final)
            *   `center;` (centrados)
            *   `space-between;` (espacio entre ellos, pegados a los bordes)
            *   `space-around;` (espacio alrededor, con medio espacio en los bordes)
            *   `space-evenly;` (espacio equitativo entre todos y los bordes)
        *   `align-items:` Cómo se distribuyen los elementos a lo largo del **eje secundario** (vertical si es `row`, horizontal si es `column`).
            *   `flex-start;`
            *   `flex-end;`
            *   `center;`
            *   `stretch;` (estirar para ocupar todo el espacio)
        *   `gap: 20px;`: Un espacio uniforme entre los elementos (más moderno que usar `margin` en los hijos).
    *   **En los elementos (los hijos):**
        *   `flex-grow: 1;`: El elemento puede crecer para ocupar espacio extra.
        *   `flex-shrink: 1;`: El elemento puede encogerse si no hay espacio.
        *   `flex-basis: 100px;`: El tamaño base del elemento antes de crecer/encogerse.
        *   `flex: 1;`: Es un atajo para `flex-grow: 1; flex-shrink: 1; flex-basis: 0;` (muy común).
    *   **Actividad: ¡Crea un Menú con Flexbox!**
        1.  Abre `estilos.css`.
        2.  Busca tu `<nav>` en el HTML, y el `<ul>` que tiene dentro. Vamos a hacer que esos `<li>` se pongan en fila y se centren.
        3.  Agrega este CSS:
            ```css
            nav ul {
                display: flex; /* Convierte el ul en un contenedor flex */
                justify-content: center; /* Centra los elementos (li) horizontalmente */
                list-style: none; /* Quita las viñetas por defecto de la lista */
                padding: 0; /* Quita el padding por defecto de la lista */
                margin: 0; /* Quita el margen por defecto de la lista */
                gap: 30px; /* Espacio entre los elementos del menú */
                background-color: #333; /* Fondo oscuro para el menú */
                padding: 15px;
                border-radius: 5px;
            }

            nav ul li a {
                color: white; /* Texto blanco para los enlaces del menú */
                text-decoration: none;
                font-weight: bold;
                padding: 5px 10px;
                transition: background-color 0.3s ease; /* Transición suave para el hover */
            }

            nav ul li a:hover {
                background-color: #555; /* Fondo más claro al pasar el mouse */
                border-radius: 3px;
            }
            ```
            *Guarda y actualiza.* ¡Verás tu menú horizontal y centrado! ¡Un cambio drástico con poco código!

*   #### **3.3. Taller: ¡Tarjetas de Hobbies con Flexbox! (15 min)**
    *   **Actividad:** Vamos a crear unas "tarjetas" para tus hobbies y las vamos a organizar con Flexbox.
        1.  **En tu `mi-primera-pagina.html`**, dentro de la `<section id="hobbies">`, crea un `div` contenedor para las tarjetas y luego 3 `div` más pequeños para cada hobby:
            ```html
            <!-- Dentro de la section Hobbies -->
            <h3>Mis Hobbies:</h3>
            <div class="contenedor-hobbies">
                <div class="tarjeta-hobby">
                    <h4>Videojuegos 🎮</h4>
                    <p>Me encanta pasar horas en [Tu Videojuego #1] y explorar nuevos mundos.</p>
                </div>
                <div class="tarjeta-hobby">
                    <h4>Música 🎧</h4>
                    <p>Siempre escuchando [Tu Artista favorito] o descubriendo nuevos géneros.</p>
                </div>
                <div class="tarjeta-hobby">
                    <h4>Deportes ⚽</h4>
                    <p>Los fines de semana, no hay nada mejor que un partido de micro en la cancha del barrio.</p>
                </div>
            </div>
            ```
        2.  **En tu `estilos.css`**, agrega estilos para el contenedor y las tarjetas:
            ```css
            .contenedor-hobbies {
                display: flex; /* Activa Flexbox para el contenedor */
                flex-direction: row; /* Pon las tarjetas en fila */
                justify-content: space-around; /* Distribuye las tarjetas con espacio alrededor */
                flex-wrap: wrap; /* Si no caben en una fila, que se envuelvan a la siguiente */
                gap: 20px; /* Espacio entre las tarjetas */
                margin-top: 30px;
            }

            .tarjeta-hobby {
                background-color: #ffffff;
                border: 1px solid #ddd;
                border-radius: 10px;
                padding: 20px;
                width: 30%; /* Cada tarjeta ocupa un 30% del ancho, para que quepan 3 en fila */
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
                text-align: center;
                transition: transform 0.3s ease; /* Para una animación al pasar el mouse */
            }

            .tarjeta-hobby:hover {
                transform: translateY(-5px); /* Se eleva un poquito al pasar el mouse */
            }
            ```
            *Guarda ambos archivos y actualiza.* ¡Ahora tus hobbies se ven en tarjetas bien organizadas!

---

### **Bloque 4: CSS Responsive Design - ¡Tu Web en Cualquier Celular! (Aprox. 1 hora)**

*   #### **4.1. El Reto Móvil: ¡Tu Web en cualquier Pantalla! (15 min)**
    *   **Discusión:** ¿Cuántos de ustedes usan más el celular que el computador para navegar? ¡La mayoría! Por eso, las páginas web deben verse bien en celulares, tablets y computadores grandes.
    *   **"Mobile First":** Es una estrategia de diseño donde primero se piensa en cómo se verá la página en el celular, y luego se adapta para pantallas más grandes.
    *   **El `meta viewport` (¡Recuerda esto!):** En el `head` de tu HTML, ya tienes esta línea:
        ```html
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        ```
        ¡Esta línea es CLAVE! Le dice al navegador que el ancho de la página debe ser el ancho del dispositivo (celular, tablet, etc.) y no una versión "grande" reducida.

*   #### **4.2. ¡Las Mágicas Media Queries! (30 min)**
    *   Las Media Queries son reglas CSS que solo se aplican si se cumplen ciertas condiciones (ej. "si la pantalla es de menos de 768px de ancho").
    *   **Sintaxis:**
        ```css
        @media screen and (max-width: 768px) {
            /* Pon aquí los estilos que quieres aplicar SOLO cuando la pantalla sea pequeña */
        }
        ```
        *   `@media screen`: Le dice que es para pantallas.
        *   `(max-width: 768px)`: La condición: si el ancho máximo de la pantalla es 768 píxeles o menos. (Este es un punto de corte común para tablets).
    *   **Actividad: ¡Haz tu página adaptable!**
        1.  Abre `estilos.css`.
        2.  Al final del archivo, agrega estas Media Queries:
            ```css
            /* ****************************************** */
            /* ESTILOS PARA PANTALLAS MÁS PEQUEÑAS (CELULARES) */
            /* ****************************************** */
            @media screen and (max-width: 768px) { /* Para pantallas de hasta 768px de ancho (tablets y celulares) */
                body {
                    margin: 10px; /* Reducimos el margen general */
                }

                header h1 {
                    font-size: 1.8em; /* Títulos más pequeños */
                }

                nav ul {
                    flex-direction: column; /* El menú se pone en columna en celulares */
                    gap: 10px; /* Menos espacio entre los ítems */
                    padding: 10px 5px;
                }

                nav ul li a {
                    padding: 10px;
                    display: block; /* Para que cada enlace ocupe todo el ancho disponible */
                    text-align: center;
                }

                .contenedor-hobbies {
                    flex-direction: column; /* Las tarjetas de hobbies se ponen en columna */
                    align-items: center; /* Centramos las tarjetas */
                }

                .tarjeta-hobby {
                    width: 90%; /* Cada tarjeta ocupa casi todo el ancho disponible */
                }

                img {
                    margin: 10px auto; /* Menos margen para las imágenes */
                }
            }

            /* ****************************************** */
            /* ESTILOS PARA PANTALLAS MUY MUY PEQUEÑAS (CELULARES PEQUEÑOS) */
            /* ****************************************** */
            @media screen and (max-width: 480px) { /* Para pantallas de hasta 480px de ancho */
                header h1 {
                    font-size: 1.5em; /* Título aún más pequeño */
                }
                h2, h3 {
                    font-size: 1.2em;
                }
            }
            ```
        3.  **¡Guarda `estilos.css` y actualiza tu página en el navegador!**
        4.  **¡A probar el responsive!**
            *   Si estás en Chrome, haz clic derecho en tu página y elige "Inspeccionar" (Inspect).
            *   Verás una barra de herramientas de desarrollador. Busca un ícono que parece un celular y una tablet (Device Toggle Toolbar) y haz clic en él.
            *   ¡Ahora puedes cambiar el tamaño de la pantalla y ver cómo tu página se adapta! ¡Prueba con diferentes anchos!
            *   También puedes arrastrar el borde de la ventana del navegador para ver cómo la página se ajusta.

*   #### **4.3. Cierre y Próximos Pasos (15 min)**
    *   **Recapitulando lo Aprendido:**
        *   **HTML Semántico:** Para una estructura inteligente y significativa (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<footer>`).
        *   **Google Fonts:** Para darle una pinta pro a tus textos.
        *   **Sombras (`text-shadow`, `box-shadow`):** Para darle profundidad a tus elementos.
        *   **Flexbox:** ¡Tu superpoder para organizar elementos en filas y columnas de forma fácil y eficiente! (`display: flex`, `justify-content`, `align-items`, `flex-direction`, `gap`).
        *   **Responsive Design con Media Queries:** Para que tu página se vea perfecta en cualquier celular o pantalla.
    *   **Mensaje Final:** ¡Ya no solo construyen una página, sino una página **inteligente, organizada y adaptable**! ¡Esto los pone en otro nivel como desarrolladores web!
    *   **¿Y Ahora Qué Sigue?**
        *   **Más Flexbox:** Hay muchas más propiedades para dominarlo.
        *   **CSS Grid:** Otro sistema de diseño poderoso para layouts más complejos (¡piensen en una cuadrícula!).
        *   **Formularios HTML:** Cómo crear formularios para que los usuarios ingresen datos.
        *   **¡Y el siguiente paso gigante... JavaScript!** Para que tus páginas hagan cosas interactivas, como animaciones, calculadoras, juegos, etc. ¡Ahí la cosa se pone súper chimba!

---

¡Felicitaciones, parceros! ¡Ya están creando experiencias web de verdad! ¡Sigan así, explorando y aprendiendo que el mundo digital es suyo!