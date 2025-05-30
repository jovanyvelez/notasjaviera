# ¡A Profundizar, Parceros! Entendiendo los "Qués" y los "Cómos" del Software 🕵️‍♂️📝

¡Qué hay de nuevo, futuros ingenieros e ingenieras! En la entrega pasada vimos el panorama general de cómo se crea el software, ¿se acuerdan? Desde la idea hasta que lo podemos usar. Pues bien, hoy vamos a meternos más al detalle en una parte crucial: **entender exactamente QUÉ queremos construir y CÓMO lo vamos a pedir**.

Porque una cosa es decir "quiero una app pa' escuchar música" y otra muy distinta es detallar si queremos que tenga playlists, que se pueda descargar pa' escuchar sin internet, que recomiende canciones... ¡Los detalles son la clave, mijos!

---

## 🗣️ Técnicas para "Sacarle la Sopa" al Cliente (Elicitación de Requisitos)

Imagínense que son detectives 🕵️‍♀️ o periodistas chismosos (pero con un buen propósito, ¡obvio!). La **elicitación de requisitos** es el arte de "sonsacarle" a la gente (clientes, futuros usuarios, etc.) toda la información necesaria para saber qué es lo que realmente quieren o necesitan que haga el software. ¡No es solo preguntar y ya! Hay que ser bien pilo.

Aquí algunas técnicas, como las herramientas de un buen detective:

1.  **Entrevistas (La Charladita Clave):**
    *   **¿Qué es?** Sentarse a hablar cara a cara (o por videollamada, pues) con las personas importantes del proyecto. Pueden ser individuales o grupales.
    *   **El Truco:** Llevar preguntas preparadas, pero también saber escuchar y hacer preguntas nuevas sobre la marcha. ¡Que la conversación fluya!
    *   **Ejemplo:** Entrevistar a los profes y estudiantes si queremos hacer una app para el colegio.

2.  **Cuestionarios y Encuestas (Preguntas Pa' Mucha Gente):**
    *   **¿Qué es?** Preparar un formulario con preguntas (abiertas o cerradas) y mandárselo a un montón de gente.
    *   **El Truco:** Hacer preguntas claras y concisas. Ideal para recoger opiniones de muchos usuarios a la vez.
    *   **Ejemplo:** Una encuesta online para saber qué funciones les gustaría a los hinchas en la nueva app de su equipo de fútbol.

3.  **Observación (Ver pa' Creer):**
    *   **¿Qué es?** Ir a donde la gente trabaja o hace sus cosas y mirar cómo lo hacen actualmente, sin el software nuevo. ¡Como un espía pero legal!
    *   **El Truco:** Fijarse en los problemas que tienen, en los pasos que dan, en las cosas que les quitan tiempo. A veces la gente no sabe decir lo que necesita, ¡pero viéndolos se pilla!
    *   **Ejemplo:** Observar cómo un tendero maneja su inventario manualmente para diseñar un software que le facilite la vida.

4.  **Talleres o Workshops (Lluvia de Ideas en Parche):**
    *   **¿Qué es?** Reunir a varias personas clave (clientes, usuarios, desarrolladores) en una misma sala (o sala virtual) para discutir ideas, definir problemas y proponer soluciones juntos.
    *   **El Truco:** Un buen moderador que guíe la conversación, use tableros, post-its, ¡lo que sea pa' que la creatividad fluya!
    *   **Ejemplo:** Un taller con gamers para diseñar las mecánicas de un nuevo videojuego.

5.  **Prototipos (Mostrar en Vez de Contar):**
    *   **¿Qué es?** Crear una versión muy básica y visual de la aplicación (a veces solo dibujos o maquetas interactivas) para que la gente la vea y dé su opinión.
    *   **El Truco:** No tiene que funcionar de verdad, solo mostrar cómo se vería y cómo se usaría. Ayuda a que la gente se imagine mejor el producto final.
    *   **Ejemplo:** Mostrarle al dueño de un restaurante unos pantallazos de cómo sería la app para tomar pedidos.

6.  **Análisis de Documentos Existentes (Revisar los Papeles):**
    *   **¿Qué es?** Si ya hay manuales, reportes, o sistemas viejos, revisarlos puede dar pistas importantes sobre lo que se necesita.
    *   **El Truco:** Buscar información relevante, procesos actuales, problemas documentados.
    *   **Ejemplo:** Revisar los informes de ventas del año pasado para entender qué datos necesita mostrar un nuevo software de análisis de ventas.

La idea es usar una combinación de estas técnicas, ¡no solo una! Así nos aseguramos de entender bien el "qué" antes de empezar a "echar código".

---

## 🎯 Requisitos Funcionales, No Funcionales y Atributos de Calidad: ¿Qué y Cómo?

Una vez que hemos "sonsacado" la información, tenemos que organizarla. Los requisitos se dividen principalmente en dos grandes grupos, más unos "primos" importantes:

### 1. Requisitos Funcionales (Lo que la App HACE 👍)

*   **¿Qué son?** Son las cosas que el sistema **DEBE HACER**. Describen las funciones, tareas o servicios específicos que el software le va a ofrecer al usuario. Son el "qué" del software.
*   **Piensa en:** Verbos de acción.
*   **Ejemplos pa' una app de domicilios:**
    *   El usuario **DEBE PODER** registrarse con su correo.
    *   El sistema **DEBE PERMITIR** buscar restaurantes por tipo de comida.
    *   El usuario **DEBE PODER** agregar productos al carrito de compras.
    *   El sistema **DEBE CALCULAR** el costo total del pedido, incluyendo el domicilio.
    *   El usuario **DEBE PODER** pagar con tarjeta de crédito.

### 2. Requisitos No Funcionales (CÓMO lo Hace la App 👌)

*   **¿Qué son?** Son las características que describen **CÓMO** el sistema debe realizar sus funciones. No se refieren a una función específica, sino a la calidad, el rendimiento, la seguridad, la usabilidad, etc., del sistema en general. Son el "cómo" del software.
*   **Piensa en:** Adjetivos o adverbios que califican el funcionamiento.
*   **Ejemplos pa' la misma app de domicilios:**
    *   La app **DEBE SER** rápida (ej: los resultados de búsqueda deben aparecer en menos de 2 segundos). (Rendimiento)
    *   La app **DEBE SER** fácil de usar para alguien que nunca la ha visto. (Usabilidad)
    *   Los datos de pago del usuario **DEBEN ESTAR** protegidos y encriptados. (Seguridad)
    *   La app **DEBE FUNCIONAR** bien en celulares Android y iPhone. (Portabilidad/Compatibilidad)
    *   La app **DEBE PODER** manejar 1000 usuarios conectados al mismo tiempo sin caerse. (Escalabilidad/Capacidad)

### 💎 Atributos de Calidad (Los "No Funcionales" Más Específicos)

Los **Atributos de Calidad** son, en esencia, requisitos no funcionales más detallados y medibles. Son las "cualidades" que queremos que tenga nuestro software. Algunos importantes:

*   **Rendimiento:** ¿Qué tan rápido responde? ¿Cuántos usuarios soporta? (Ej: "La página principal debe cargar en menos de 3 segundos").
*   **Usabilidad:** ¿Qué tan fácil es de aprender y usar? ¿Es intuitivo? (Ej: "Un nuevo usuario debe poder hacer un pedido en menos de 5 minutos sin ayuda").
*   **Fiabilidad (Reliability):** ¿Qué tan seguido falla? ¿Se recupera fácil de los errores? (Ej: "El sistema debe estar disponible el 99.9% del tiempo").
*   **Seguridad:** ¿Qué tan protegido está contra ataques o accesos no autorizados? (Ej: "Las contraseñas deben almacenarse encriptadas").
*   **Mantenibilidad:** ¿Qué tan fácil es de corregir, adaptar o mejorar en el futuro? (Ej: "El código debe estar bien comentado y ser modular").
*   **Portabilidad:** ¿Qué tan fácil es de llevar a otros ambientes (otro sistema operativo, otro servidor)? (Ej: "La app debe funcionar en Windows y Linux").

Entender bien la diferencia entre funcionales y no funcionales es clave. ¡De nada sirve una app que hace mil cosas (funcionales) si es lentísima, se cae a cada rato o nadie la entiende (no funcionales malos)!

---

## 🎬 Casos de Uso: La "Película" de Cómo Interactúas con la App

Un **Caso de Uso** es como el guion de una película corta que describe una interacción específica entre un **actor** (una persona, otro sistema, o incluso el tiempo) y el software para lograr un **objetivo**. ¡Es contar una historia de cómo se usa el sistema!

*   **Actor:** ¿Quién inicia la acción o interactúa con el sistema? (Ej: Cliente, Administrador, Sistema de Pagos).
*   **Objetivo:** ¿Qué quiere lograr el actor? (Ej: Registrarse, Comprar un producto, Generar un reporte).

**¿Para qué sirven?**

*   Ayudan a entender mejor qué necesita hacer el sistema desde la perspectiva del usuario.
*   Son una forma clara de comunicar los requisitos funcionales.
*   Sirven de base para diseñar y probar el software.

**Ejemplo sencillo de un Caso de Uso (en texto, aunque a veces se dibujan):**

*   **Nombre del Caso de Uso:** Realizar Compra Online.
*   **Actor Principal:** Cliente.
*   **Resumen:** El Cliente selecciona productos, los agrega al carrito, proporciona datos de envío y pago, y confirma la compra.
*   **Flujo Básico (Pasos Principales):**
    1.  El Cliente navega por el catálogo de productos.
    2.  El Cliente selecciona un producto y lo añade al carrito.
    3.  El Cliente va al carrito de compras.
    4.  El Sistema muestra los productos en el carrito y el total.
    5.  El Cliente procede al pago.
    6.  El Cliente ingresa sus datos de envío.
    7.  El Cliente selecciona un método de pago e ingresa los datos.
    8.  El Sistema valida el pago.
    9.  El Sistema confirma la compra y muestra un resumen del pedido.
*   **Flujos Alternativos (¿Qué pasa si algo sale mal o diferente?):**
    *   El producto seleccionado no tiene stock.
    *   El pago es rechazado.
    *   El cliente quiere cancelar un producto del carrito.

Los casos de uso son súper útiles porque nos obligan a pensar en todos los pasos y posibles situaciones.

---

## 📚 Documentación de Requisitos: ¡Que no se Nos Olvide Nada!

Imagínate construir una casa sin planos detallados, solo con ideas en la cabeza. ¡Sería un desastre! La **documentación de requisitos** es como esos planos para el software. Es el proceso de escribir, de forma clara y organizada, todos los requisitos funcionales, no funcionales, casos de uso, y cualquier otra información importante sobre lo que el software debe hacer.

**¿Por qué es tan importante este "papelerío"?**

*   **Claridad para todos:** Asegura que tanto el cliente como el equipo de desarrollo tengan la misma película en la cabeza. ¡Evita malentendidos!
*   **Guía para el desarrollo:** Los programadores la usan como su biblia para saber qué construir.
*   **Base para las pruebas:** Los testers (QA) la usan para saber qué probar y si el software cumple con lo prometido.
*   **Control de cambios:** Si alguien quiere cambiar algo, se puede ver cómo afecta a los requisitos ya definidos.
*   **Memoria del proyecto:** Si alguien nuevo llega al equipo o si se retoma el proyecto después de un tiempo, la documentación es oro.

**¿Qué se incluye normalmente?**

*   Una introducción y descripción general del proyecto.
*   Lista detallada de requisitos funcionales.
*   Lista detallada de requisitos no funcionales (y atributos de calidad).
*   Casos de uso (descritos o a veces con diagramas).
*   Modelos visuales (prototipos, mockups, diagramas de flujo, etc.).
*   Un glosario de términos (pa' que todos hablen el mismo idioma).

El documento más famoso donde se plasma todo esto se llama **SRS (Software Requirements Specification)** o Especificación de Requisitos del Software. ¡Es como la cédula del proyecto!

---

## 📜 Creación y Priorización de Historias de Usuario: ¡Pequeñas Misiones Claras!

En las metodologías ágiles (como Scrum), en vez de documentos gigantescos de requisitos, se suele trabajar con **Historias de Usuario**. Son una forma más sencilla y amigable de describir una funcionalidad desde la perspectiva de quien la va a usar.

**¿Cómo se escribe una Historia de Usuario?**

Siguen un formato bien chévere:

**"Como un [ROL/TIPO DE USUARIO], quiero [ACCIÓN/FUNCIONALIDAD] para poder [BENEFICIO/OBJETIVO]."**

**Ejemplos:**

*   **"Como un *cliente registrado*, quiero *guardar mis direcciones de envío* para poder *hacer pedidos más rápido la próxima vez*."**
*   **"Como un *administrador del blog*, quiero *aprobar o rechazar comentarios* para poder *mantener un ambiente respetuoso*."**
*   **"Como un *jugador nuevo*, quiero *ver un tutorial corto al iniciar el juego* para poder *entender las mecánicas básicas rápidamente*."**

**¿Por qué son tan bacanas las Historias de Usuario?**

*   **Enfocadas en el usuario:** Ponen las necesidades del usuario en el centro.
*   **Fáciles de entender:** Son cortas, claras y cualquiera las pilla.
*   **Promueven la conversación:** No son contratos, son recordatorios para hablar más a fondo sobre la funcionalidad.
*   **Tamaño manejable:** Se pueden completar en un ciclo corto de desarrollo (Sprint).

**¡A Priorizar, que no todo cabe en la maleta! (Priorización)**

Una vez que tenemos un montón de historias de usuario (o requisitos en general), ¡no podemos hacerlas todas a la vez! Hay que decidir qué es lo más importante, qué va primero. Eso es **priorizar**.

Algunas formas de priorizar (hay muchas, pero estas son comunes):

1.  **MoSCoW (El Deber Ser, el Debería, el Podría, el No Hará... por ahora):**
    *   **M - Must have (Debe Tener):** ¡Súper crítico! Si no está, el producto no sirve o no se puede lanzar. (Ej: En una app de chat, poder enviar mensajes).
    *   **S - Should have (Debería Tener):** Importante, pero no vital para el lanzamiento. Se puede vivir sin ello temporalmente. (Ej: Enviar emojis).
    *   **C - Could have (Podría Tener):** Deseable, pero menos importante. Un "lujito" si hay tiempo. (Ej: Cambiar el color del chat).
    *   **W - Won't have (No Tendrá):** Cosas que se decide explícitamente NO hacer en esta versión (quizás más adelante).

2.  **Valor vs. Esfuerzo (Lo que más Paga con Menos Camello):**
    *   Se evalúa cada historia por el **valor** que le da al negocio o al usuario y por el **esfuerzo** (tiempo, costo) que toma desarrollarla.
    *   Se busca hacer primero lo que da mucho valor con poco esfuerzo.

3.  **Numeración Simple (1, 2, 3...):**
    *   Simplemente ordenar las historias de la más importante a la menos importante.

La priorización la suele liderar el **Product Owner** (en Scrum) o el cliente, con la ayuda del equipo para entender el esfuerzo.

---

## 🚀 ¡Listos pa' Pedir lo que Quieren (y que se los Entiendan)!

¡Ahí lo tienen, parceros! Ahora saben cómo los equipos de software se las ingenian para entender a la perfección qué es lo que se necesita construir. Desde las técnicas de detective para sacar la información, hasta cómo escribir y organizar esos pedidos para que no haya pierde.

Conocer los requisitos funcionales, no funcionales, los casos de uso y las historias de usuario es como tener el mapa del tesoro antes de empezar la aventura de desarrollar.

¡Sigan así de curiosos y preguntones! El mundo del software los espera con los brazos abiertos. ¿Alguna duda? ¡De una, pregunten en los comentarios! Nos pillamos en la próxima. 🤘