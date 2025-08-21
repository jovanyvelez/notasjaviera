# Curso "¡Pura Pinta Web!" 💻✨
## Crea tus Primeras Páginas con HTML y CSS (¡Sin Enredos con JavaScript por Ahora!)

**Para:** Jóvenes de grado diez de la Javiera Londoño de Medellín, Antioquia.
**Duración Estimada:** Unas 4 horas de parche y código (¡pero a tu ritmo!).
**Nivel:** Desde cero, ¡aquí todos empezamos a programar!

---

### **📝 Nota Importante para Navegar este Archivo:**

Este documento es como su mapa del tesoro para el mundo web.
*   **Lee con calma:** No te afanes, cada concepto es un ladrillo para construir tu página.
*   **Haz las actividades:** Son la clave para que el conocimiento se te quede en la cabeza y en las manos. Puedes hacer los códigos en tu computador y ver cómo quedan.
*   **No te asustes con el inglés:** El mundo de la programación habla inglés, pero aquí te lo explicamos en paisa.
*   **¡Experimenta!** Cambia valores, prueba cosas diferentes. ¡Así es como se aprende de verdad!
*   **¡Pregunta!** Si estás en un grupo, discutan las dudas. Si estás solo, anota tus preguntas para cuando tengas la oportunidad de hablar con alguien que sepa.
*   **¡Diviértete!** Ver tu primera página web nacer es una sensación muy chimba.

---

## 🎯 **Objetivos de este Parche Web:**

Al final de este curso, vas a estar un "teso" (o "tesa") en la creación web básica, capaz de:
*   Entender qué es **HTML** y para qué sirve (¡el esqueleto de tu página!).
*   Entender qué es **CSS** y para qué sirve (¡la ropa y el maquillaje de tu página!).
*   Crear tu primera página web con texto, imágenes y enlaces.
*   Darle estilo y color a tu página para que se vea bien bacana.
*   Guardar y abrir tus archivos web en cualquier navegador.

---

## 📚 **¿Qué Necesitas para este Parche de Programación?**

*   Tu computador (¡obvio!).
*   Un **editor de código**. Te recomendamos **VS Code** (Visual Studio Code). Es gratis, fácil de usar y el más popular. ¡Búscalo en Google y descárgalo!
*   Un navegador web (Chrome, Firefox, Edge, Safari).
*   Ganas de aprender y crear cosas ¡muy chimba!

---

## ⏰ **¡A Ponerle Ambiente a la Clase! (Organización por Bloques)**

---

### **Bloque 1: HTML - El Esqueleto de tu Página (Aprox. 1 hora)**

*   #### **1.1. ¡Hola, Mundo Web! ¿Qué es HTML? (15 min)**
    *   **¿Qué es?** HTML significa **H**yper**T**ext **M**arkup **L**anguage. ¡Uy, qué nombre tan largo! Pero tranquilos, es como si fuera un "lenguaje de marcado".
    *   **¿Para qué sirve?** Piensen que una página web es como una casa. **HTML es el esqueleto de esa casa:** las paredes, los techos, las puertas, las ventanas. Define la **estructura** y el **contenido**.
    *   **¡No es un lenguaje de programación!** HTML no hace cálculos ni toma decisiones. Solo le dice al navegador: "esto es un título", "esto es un párrafo", "aquí va una imagen".
    *   **Las "etiquetas" (Tags):** HTML funciona con etiquetas. Las etiquetas son como "instrucciones" encerradas entre `< >`. La mayoría vienen en pares: una de apertura y una de cierre.
        *   `<h1> Esto es un título grande </h1>`
        *   `<p> Esto es un párrafo de texto. </p>`

*   #### **1.2. La Estructura Básica de Toda Página (20 min)**
    *   Toda página HTML tiene una estructura fija, como el cuerpo humano tiene cabeza, tronco y extremidades.
    *   **¡Abre VS Code y crea tu primer archivo!**
        1.  Abre VS Code.
        2.  Ve a `Archivo` (File) -> `Nuevo Archivo de Texto` (New Text File).
        3.  Ve a `Archivo` (File) -> `Guardar Como` (Save As...).
        4.  Dale un nombre: `mi-primera-pagina.html` (¡la extensión `.html` es CLAVE!). Guárdalo en una carpeta que encuentres fácil.
    *   **Copia y pega este código en tu `mi-primera-pagina.html`:**
        ```html
        <!DOCTYPE html>
        <html lang="es">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Mi Perfil Bacano en la Web</title>
        </head>
        <body>

            <!-- Aquí es donde va todo el contenido que vas a ver en la página -->
            <h1>¡Hola, Parceros! Soy [Tu Nombre]</h1>
            <p>Bienvenidos a mi primera página web. ¡Estoy aprendiendo HTML!</p>

        </body>
        </html>
        ```
    *   **Guarda el archivo** (`Ctrl+S` o `Cmd+S`).
    *   **¡Mira tu página en el navegador!** Busca el archivo `mi-primera-pagina.html` en la carpeta donde lo guardaste y haz doble clic sobre él. ¡Se abrirá en tu navegador!
    *   **Explicando la estructura:**
        *   `<!DOCTYPE html>`: Le dice al navegador que es un documento HTML5 (la versión más reciente).
        *   `<html lang="es">`: Es la etiqueta principal que envuelve todo el contenido. `lang="es"` le dice que el idioma de la página es español.
        *   `<head>`: Es la "cabeza" de la página. Aquí va información que el usuario *no ve directamente*, pero que es importante para el navegador (ej. el título de la pestaña, la configuración de caracteres).
            *   `<meta charset="UTF-8">`: Para que los tildes y las "ñ" se vean bien.
            *   `<meta name="viewport" ...>`: Para que la página se vea bien en celulares y tablets.
            *   `<title>Mi Perfil Bacano en la Web</title>`: ¡Este es el texto que aparece en la pestaña del navegador!
        *   `<body>`: ¡Este es el "cuerpo" de la página! **Todo lo que ves en la pantalla va aquí dentro.**
        *   `<!-- Esto es un comentario -->`: Los comentarios no se ven en la página, solo sirven para que tú o otros programadores entiendan el código.

*   #### **1.3. Agregando Contenido: Títulos, Párrafos y Enlaces (25 min)**
    *   **Títulos (`<h1>` a `<h6>`):** Sirven para organizar el contenido. `<h1>` es el más grande e importante, `<h6>` el más pequeño.
        *   **Actividad:** Dentro del `<body>` de tu `mi-primera-pagina.html`, cambia y agrega:
            ```html
            <h1>¡Hola, Parceros! Soy [Tu Nombre]</h1>
            <h2>Sobre Mí:</h2>
            <p>Nací en [Tu Barrio o Ciudad] y vivo en [Tu Barrio o Ciudad]. Me gusta mucho [Tu Hobby o Deporte favorito].</p>
            <h3>Mis Hobbies:</h3>
            <p>Además de [Tu Hobby anterior], me encanta [Otro Hobby], y también disfruto [Un Hobby más].</p>
            ```
            *Guarda el archivo y actualiza la página en el navegador para ver los cambios.*

    *   **Enlaces (`<a>`): ¡Para ir a otras páginas!**
        *   La etiqueta `<a>` (de "anchor", ancla) sirve para crear hipervínculos (links).
        *   Necesita un **atributo `href`** (de "hypertext reference") que le dice a dónde ir.
        *   También puedes usar el atributo `target="_blank"` para que el enlace se abra en una nueva pestaña.
        *   **Actividad:** Agrega estos enlaces debajo de tus párrafos:
            ```html
            <p>Puedes visitar <a href="https://www.medellin.gov.co/" target="_blank">la página oficial de Medellín</a> para saber más de mi ciudad.</p>
            <p>Si te interesa la tecnología, te recomiendo <a href="https://developer.mozilla.org/es/docs/Web" target="_blank">MDN Web Docs</a>.</p>
            ```
            *Guarda y prueba los enlaces en tu navegador.*

---

### **Bloque 2: HTML - ¡Más Carne al Esqueleto! Imágenes y Listas (Aprox. 1 hora)**

*   #### **2.1. ¡Pura Imagen! Agregando Fotos (25 min)**
    *   Las imágenes hacen que una página sea mucho más atractiva. La etiqueta para imágenes es `<img>`.
    *   **¡OJO!** La etiqueta `<img>` no tiene etiqueta de cierre (`</img>`). Es una de las pocas excepciones.
    *   Necesita dos atributos CLAVE:
        *   `src` (de "source"): La dirección donde está la imagen. Puede ser una dirección de internet o una ruta a una imagen que tengas en tu computador.
        *   `alt` (de "alternative text"): Un texto que describe la imagen. Esto es importante por si la imagen no carga, o para personas con discapacidad visual.
    *   **Actividad: Agrega una imagen a tu página.**
        1.  **Opción A (Imagen de Internet):** Busca una imagen en Google (ej. "Medellín aerial view"). Haz clic derecho sobre la imagen y elige "Copiar dirección de imagen" (Copy image address). Pégala en el `src`.
        2.  **Opción B (Imagen tuya):** Pon una foto tuya o de algo que te guste en la misma carpeta donde tienes tu archivo `mi-primera-pagina.html`. Por ejemplo, si tu foto se llama `mi_foto.jpg`.
        3.  **Agrega el código en tu `<body>`:**
            ```html
            <h2>Mi Foto (o una foto de algo que me guste):</h2>
            <!-- Si usas una imagen de internet -->
            <img src="URL_DE_TU_IMAGEN_DE_INTERNET" alt="Vista aérea de Medellín">
            <!-- Si usas una imagen de tu computador (asegúrate que el nombre y la extensión sean correctos) -->
            <!-- <img src="mi_foto.jpg" alt="Mi foto personal"> -->

            <p>¡Aquí estoy yo! (o la imagen de tu lugar favorito de Medellín).</p>
            ```
            *Guarda y actualiza para ver tu imagen.*

*   #### **2.2. ¡Listas para todo! Organizadores de Contenido (20 min)**
    *   Las listas son súper útiles para presentar información de forma organizada. Hay dos tipos principales:
        *   **Listas Desordenadas (`<ul>` - Unordered List):** Son listas con viñetas (puntos, cuadrados, etc.).
        *   **Listas Ordenadas (`<ol>` - Ordered List):** Son listas numeradas.
    *   Dentro de `<ul>` o `ol`, cada elemento de la lista va con la etiqueta `<li>` (List Item).
    *   **Actividad: ¡Crea algunas listas sobre tus gustos!**
        *   **Mis Comidas Favoritas (Desordenada):**
            ```html
            <h3>Mis Comidas Favoritas:</h3>
            <ul>
                <li>Bandeja Paisa</li>
                <li>Arepa con Hogao</li>
                <li>Empanadas (¡obvio!)</li>
                <li>Salchipapa</li>
            </ul>
            ```
        *   **Mis Videojuegos Top (Ordenada):**
            ```html
            <h3>Mis Videojuegos Top 3:</h3>
            <ol>
                <li>[Tu Videojuego #1]</li>
                <li>[Tu Videojuego #2]</li>
                <li>[Tu Videojuego #3]</li>
            </ol>
            ```
            *Guarda y actualiza para ver tus listas.*

*   #### **2.3. Contenedores: `<div>` y `<span>` (15 min)**
    *   Estas etiquetas son como "cajas" para organizar tu contenido, especialmente cuando queremos aplicar estilos con CSS.
        *   **`<div>` (Division):** Es una "caja" de bloque. ¡Imagina que es una sección completa de tu página, como un cajón grande! Cada `<div>` nuevo se pone debajo del anterior.
        *   **`<span>`:** Es una "caja" en línea. ¡Imagina que es solo para una palabra o una frase corta dentro de un párrafo! No crea una nueva línea.
    *   **Actividad:** No vamos a ver efectos ahora, pero vamos a usarlas para que te acostumbres.
        *   Envuelve tu sección "Sobre Mí" en un `<div>`:
            ```html
            <div class="seccion-sobre-mi">
                <h2>Sobre Mí:</h2>
                <p>Nací en [Tu Barrio o Ciudad] y vivo en [Tu Barrio o Ciudad]. Me gusta mucho [Tu Hobby o Deporte favorito].</p>
            </div>
            ```
        *   Marca una palabra con `<span>`:
            ```html
            <p>Bienvenidos a mi <span class="destacado">primera página web</span>. ¡Estoy aprendiendo HTML!</p>
            ```
            *Guarda. No verás cambios visuales aún, ¡pero ya tienes las "cajas" listas para CSS!*

---

### **Bloque 3: CSS - ¡La Pinta de tu Página! (Aprox. 1 hora)**

*   #### **3.1. ¿Qué es CSS? ¡El Diseñador de Modas de tu Web! (15 min)**
    *   **¿Qué es?** CSS significa **C**ascading **S**tyle **S**heets (Hojas de Estilo en Cascada).
    *   **¿Para qué sirve?** Si HTML es el esqueleto de la casa, **CSS es la pintura, los muebles, la decoración, el color de las paredes.** ¡Le da el estilo y la pinta a tu página!
    *   **Separación de Cuentas:** Es una buena práctica tener el HTML y el CSS en archivos separados. Así el código está más ordenado.
    *   **Reglas CSS:** Funciona con "reglas" que le dicen a qué elemento aplicar un estilo, y qué estilo aplicar.
        ```css
        selector {
            propiedad: valor;
            propiedad2: valor2;
        }
        ```
        *   **`selector`:** A quién le vas a aplicar el estilo (ej. `h1`, `p`, `.destacado`).
        *   **`propiedad`:** Qué quieres cambiar (ej. `color`, `font-size`, `background-color`).
        *   **`valor`:** Cómo quieres cambiarlo (ej. `blue`, `24px`, `#f0f0f0`).

*   #### **3.2. Conectando tu CSS y HTML (15 min)**
    *   **Crea tu archivo CSS:**
        1.  En VS Code, ve a `Archivo` (File) -> `Nuevo Archivo de Texto` (New Text File).
        2.  `Archivo` (File) -> `Guardar Como` (Save As...).
        3.  Dale un nombre: `estilos.css` (¡la extensión `.css` es CLAVE!). Guárdalo en la *misma carpeta* que `mi-primera-pagina.html`.
    *   **Conecta HTML con CSS:** Para que tu HTML se entere de que existe tu archivo CSS, tienes que "linkearlo" en la sección `<head>` de tu `mi-primera-pagina.html`.
        *   **Abre `mi-primera-pagina.html`** y justo antes de `</head>`, agrega esta línea:
            ```html
            <link rel="stylesheet" href="estilos.css">
            ```
        *   `rel="stylesheet"`: Le dice que es una hoja de estilos.
        *   `href="estilos.css"`: Le dice dónde encontrar tu archivo CSS (como está en la misma carpeta, solo pones el nombre).
        *   *Guarda los cambios en `mi-primera-pagina.html`.*

*   #### **3.3. Dándole Estilo: Selectores y Propiedades Básicas (30 min)**
    *   **Selectores:**
        *   **Selector de Etiqueta:** Aplica el estilo a *todas* las etiquetas de ese tipo. (Ej: `h1`, `p`, `img`).
        *   **Selector de Clase:** Para aplicar estilos a elementos específicos. Los defines con el atributo `class="nombre-de-clase"` en HTML y los seleccionas con un punto `.` en CSS (Ej: `.destacado`).
        *   **Selector de ID:** Para un solo elemento ÚNICO en toda la página. Los defines con el atributo `id="nombre-de-id"` en HTML y los seleccionas con un numeral `#` en CSS (Ej: `#mi-titulo-principal`).
    *   **Propiedades y Valores (¡A probar en `estilos.css`!):**
        *   **Colores:** `color` (texto), `background-color` (fondo). Puedes usar nombres de colores (red, blue, green) o códigos hexadecimales (`#FF0000` para rojo, `#0000FF` para azul).
        *   **Tamaño de Fuente:** `font-size` (ej: `16px`, `1.2em`).
        *   **Tipo de Fuente:** `font-family` (ej: `Arial, sans-serif`).
        *   **Alineación de Texto:** `text-align` (`left`, `center`, `right`).
    *   **Actividad: ¡Dale color y estilo a tu página!**
        *   **Abre `estilos.css`** y pega este código:
            ```css
            body { /* Aplica a todo el cuerpo de la página */
                font-family: Arial, sans-serif; /* Un tipo de letra simple */
                background-color: #f0f0f0; /* Un gris claro para el fondo */
                color: #333; /* Un gris oscuro para el texto */
                margin: 20px; /* Un pequeño margen alrededor de todo el contenido */
            }

            h1 {
                color: #2c3e50; /* Un azul oscuro */
                text-align: center; /* Centrar el título */
                border-bottom: 2px solid #3498db; /* Una línea azul debajo del título */
                padding-bottom: 10px; /* Espacio entre el texto y la línea */
            }

            h2 {
                color: #3498db; /* Un azul más claro */
            }

            p {
                line-height: 1.6; /* Espacio entre líneas para que se lea mejor */
            }

            a {
                color: #e74c3c; /* Un rojo para los enlaces */
                text-decoration: none; /* Quitar el subrayado de los enlaces */
            }

            a:hover { /* Cuando pasas el mouse por encima del enlace */
                text-decoration: underline; /* Aparece el subrayado */
            }

            img {
                max-width: 100%; /* Para que la imagen no se salga de la pantalla en celulares */
                height: auto; /* Para que la altura se ajuste automáticamente */
                border: 5px solid #2ecc71; /* Un borde verde para la imagen */
                border-radius: 10px; /* Bordes redondeados */
                display: block; /* Para que la imagen se comporte como un bloque y el texto no la rodee */
                margin: 20px auto; /* Para centrar la imagen y darle espacio */
            }

            ul, ol {
                background-color: #ecf0f1; /* Un gris muy claro para el fondo de las listas */
                padding: 20px; /* Espacio interno de la caja de la lista */
                border-left: 5px solid #9b59b6; /* Una línea morada a la izquierda */
            }

            .destacado { /* Estilo para la clase "destacado" que pusimos en el <span> */
                font-weight: bold; /* Texto en negrilla */
                color: #f39c12; /* Un naranja vibrante */
            }

            /* Aquí podemos darle estilo a la caja div que creamos */
            .seccion-sobre-mi {
                background-color: #fff; /* Fondo blanco */
                padding: 20px; /* Espacio interno */
                margin-bottom: 20px; /* Espacio debajo de la caja */
                border-radius: 8px; /* Bordes redondeados */
                box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Una pequeña sombra para que parezca una tarjeta */
            }
            ```
            *Guarda `estilos.css` y actualiza `mi-primera-pagina.html` en tu navegador. ¡Verás cómo cambió toda la pinta!*

---

### **Bloque 4: ¡Pura Pinta Profesional! Más CSS y un Mini-Proyecto (Aprox. 1 hora)**

*   #### **4.1. El Modelo de Caja: ¡Todo es una Caja! (25 min)**
    *   En diseño web, ¡todo lo que ves es una caja! Un párrafo, una imagen, un título, ¡todo! Y estas cajas tienen propiedades importantes:
        *   **Content (Contenido):** El texto, la imagen, etc.
        *   **Padding (Relleno):** El espacio *dentro* de la caja, entre el contenido y el borde.
        *   **Border (Borde):** La línea que rodea la caja.
        *   **Margin (Margen):** El espacio *fuera* de la caja, entre la caja y otros elementos.
    *   **Piensa en una caja de regalo:**
        *   El regalo es el **contenido**.
        *   El papel de seda *dentro* de la caja es el **padding**.
        *   La caja misma es el **border**.
        *   El espacio entre tu caja y otras cajas en la mesa es el **margin**.
    *   **Propiedades en CSS:**
        *   `padding: 10px;` (o `padding-top`, `padding-right`, `padding-bottom`, `padding-left`)
        *   `border: 2px solid black;` (grosor, estilo, color)
        *   `margin: 20px;` (o `margin-top`, etc.)
        *   También `width` (ancho) y `height` (alto).
    *   **¡Experimenta con el Modelo de Caja!**
        *   Vuelve a tu `estilos.css`. Busca el selector `p { ... }`.
        *   Agrega y juega con estas propiedades, guarda y mira los cambios en el navegador:
            ```css
            p {
                line-height: 1.6;
                /* Prueba esto: */
                border: 1px dashed gray; /* Un borde punteado gris */
                padding: 15px; /* Relleno interno */
                margin-bottom: 25px; /* Margen externo debajo */
                background-color: lightyellow; /* Fondo amarillo claro solo para los párrafos */
            }
            ```
            *¡Puedes ver cómo cada párrafo se convierte en una caja con sus propios espacios!*

*   #### **4.2. ¡Proyecto Final Sencillo! "Mi Parche en Medellín" (50 min)**
    *   **Objetivo:** Crear una nueva página sobre tu lugar favorito o tu parche en Medellín, aplicando todo lo aprendido.
    *   **Pasos:**
        1.  **Crea un nuevo archivo HTML:** `mi-parche-medellin.html`.
        2.  **Crea un nuevo archivo CSS:** `estilos-parche.css`.
        3.  **Linkea** `estilos-parche.css` en la sección `<head>` de `mi-parche-medellin.html`.
        4.  **Piensa en tu lugar favorito:** ¿El Parque Lleras? ¿Plaza Botero? ¿Parque Explora? ¿La Unidad Deportiva Atanasio Girardot?
        5.  **Estructura con HTML (`mi-parche-medellin.html`):**
            *   Un `<h1>` con el nombre de tu lugar.
            *   Un párrafo `<p>` describiendo por qué te gusta.
            *   Una imagen `<img>` del lugar (búscala en internet).
            *   Una lista `<ul>` con 3-5 razones por las que es tu parche.
            *   Un enlace `<a>` a Google Maps con la ubicación.
            *   ¡Usa al menos un `<div>` y un `<span>` para agrupar contenido!
            *   ¡Agrega comentarios `<!-- -->` para explicar secciones de tu código!
        6.  **Dale estilo con CSS (`estilos-parche.css`):**
            *   Cambia el `background-color` del `body`.
            *   Personaliza los colores de tus títulos (`h1`, `h2`, etc.) y párrafos.
            *   Dale un `border`, `padding` y `margin` a tu `<div>` principal.
            *   Haz que la imagen se vea bien ( `max-width: 100%; height: auto;`).
            *   Estiliza tus listas (puedes cambiar el tipo de viñeta con `list-style-type`).
            *   Cambia el estilo de tus enlaces (`a`).
            *   ¡Usa tus clases (`.`) para darle un estilo especial a alguna frase o sección!
    *   **¡Guarda todo y abre `mi-parche-medellin.html` en tu navegador!** ¡Siente el orgullo de ver tu propia página diseñada por ti!

*   #### **4.3. Cierre y Próximos Pasos (5 min)**
    *   **Recapitulando lo Aprendido:**
        *   **HTML:** La estructura, el esqueleto, con sus etiquetas para títulos, párrafos, imágenes, enlaces y listas.
        *   **CSS:** El diseño, la pinta, el maquillaje, con sus selectores y propiedades para colores, fuentes y espacios.
        *   ¡Ambos trabajan juntos para crear una página web bacana!
    *   **Mensaje Final:** ¡Acaban de dar sus primeros pasos en el mundo de la creación web! Esto es como aprender a montar en cicla: al principio es raro, pero con práctica se vuelve muy fácil y divertido.
    *   **¿Y Ahora Qué Sigue?**
        *   **¡Practica!** Intenta crear más páginas, ¡o mejora las que ya hiciste!
        *   **Aprende más CSS:** Hay un mundo de propiedades para posicionar elementos, animaciones, diseños responsivos (que se ven bien en cualquier pantalla).
        *   **Descubre JavaScript:** En un futuro curso, veremos cómo darle "vida" a tus páginas, que hagan cosas interactivas, cálculos, etc. ¡Ahí sí es un lenguaje de programación de verdad!
        *   **Explora:** ¡Mira el código fuente de tus páginas favoritas! (En el navegador, haz clic derecho y elige "Ver código fuente de la página" o "Inspeccionar").

---

¡Felicitaciones, futuros desarrolladores web de Medellín! ¡Están construyendo el internet del mañana! ¡Pilas pues, que esto apenas empieza!