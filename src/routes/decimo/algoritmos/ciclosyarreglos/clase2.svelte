<script>
// No se requiere lógica JS para este contenido, todo es visual
</script>

<main class="clase2-container">
  <section class="intro">
    <h1>¡Hey, Parceros y Parceras Programadoras de Medallo! 🚀</h1>
    <p class="bienvenida">¡Qué más pues! Bienvenidos a esta nueva aventura donde vamos a aprender unos trucos súper poderosos para que sus programas hagan cosas increíbles. Hoy vamos a hablar de <b>Ciclos</b> y <b>Arreglos</b>. Suena como a cosa de nerds, ¿cierto? ¡Pero qué va! Es más fácil de lo que creen y les va a servir pa' un montón de cosas, desde organizar la música de su celular hasta crear sus propios juegos.</p>
    <p>Imaginen que van a hacer un sancocho bien delicioso pa' invitar a todo el combo de amigos. Hay tareas que se repiten, ¿o qué? Como picar la yuca, la papa, el plátano... ¡Uff! Y también necesitan una lista de todos los ingredientes pa' que no se les olvide nada. Bueno, los ciclos y los arreglos nos ayudan con eso en el mundo de la programación.</p>
    <div class="destacado">¿Listos pa' poner al computador a camellar por ustedes? <b>¡Empecemos!</b></div>
  </section>

  <section class="ciclos">
    <h2>⚙️ ¿Qué Son los Ciclos? - Poniendo al Computador a "Camellar" por Vos</h2>
    <ul>
      <li>Escuchar esa canción de Feid o Karol G que no se les sale de la cabeza... ¡en bucle!</li>
      <li>Darle vueltas a la cancha de fútbol del barrio pa' calentar.</li>
      <li>Cuando la abuela les dice: "Mijo, salúdeme a toda la familia", y ustedes empiezan: "Hola tía...", "Hola primo...", y así con cada uno.</li>
    </ul>
    <p>En programación, un <b>ciclo</b> (o bucle) es simplemente una forma de decirle al computador: <span class="frase">¡Parcero, repetí esta tarea varias veces!</span> Así no tenemos que escribir el mismo código mil veces. ¡El computador lo hace por nosotros!</p>
    <p>Hay dos tipos principales de ciclos que vamos a ver, como tener dos rutas distintas pa' llegar al Poblado: el ciclo <b>for</b> y el ciclo <b>while</b>.</p>
  </section>

  <section class="for-section">
    <h3>🔁 El Ciclo <code>for</code>: Cuando Sabés Cuántas Vueltas Dar</h3>
    <p>El ciclo <b>for</b> es el que usamos cuando sabemos <b>exactamente cuántas veces</b> queremos que se repita algo. Es como cuando el profe de educación física dice: <span class="frase">¡Cinco vueltas a la cancha, pues!</span> Sabés que son 5, ni más ni menos.</p>
    <ul>
      <li>Quieren enviar un mensaje de "Feliz Navidad, parcero" a sus 10 mejores amigos. Saben que son 10 mensajes.</li>
      <li>Quieren contar los pisos de un edificio que tiene 20 pisos.</li>
    </ul>
    <div class="codigo">
      <div class="codigo-titulo">¿Cómo se ve esto en C#?</div>
      <pre><code>{`for (int i = 1; i <= 5; i++) {
    Console.WriteLine("¡Hola, futuro programador de Medallo! Saludo número: " + i);
}`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`¡Hola, futuro programador de Medallo! Saludo número: 1
¡Hola, futuro programador de Medallo! Saludo número: 2
¡Hola, futuro programador de Medallo! Saludo número: 3
¡Hola, futuro programador de Medallo! Saludo número: 4
¡Hola, futuro programador de Medallo! Saludo número: 5`}</code></pre>
    </div>
    <div class="ejemplo-paisa">
      <b>Ejemplo bien paisa con <code>for</code>:</b>
      <p>Vamos a simular que estamos anunciando las estaciones de la Línea A del Metro, desde Niquía hasta La Estrella (vamos a poner solo algunas pa' no alargar mucho).</p>
      <div class="codigo-responsive">
        <pre><code>{`string[] estacionesMetro = {\
  "Niquía", "Bello", "Madera", "Acevedo",\
  "Caribe", "San Antonio", "Poblado",\
  "Envigado", "Itagüí", "La Estrella"\
};\nfor (int i = 0; i < estacionesMetro.Length; i++) {\n    Console.WriteLine("Próxima estación: " + estacionesMetro[i]);\n}`}</code></pre>
      </div>
    </div>
  </section>

  <section class="while-section">
    <h3>🔄 El Ciclo <code>while</code>: Mientras Haya Aguardiente en la Botella...</h3>
    <p>El ciclo <b>while</b> es diferente. Este lo usamos cuando queremos que algo se repita <b>mientras una condición sea verdadera</b>, pero no sabemos exactamente cuántas veces va a ser.</p>
    <ul>
      <li>Jugar parqués hasta que alguien gane. ¿Cuántas rondas serán? ¡Quién sabe! Se juega <b>mientras</b> nadie haya ganado.</li>
      <li>Comer empanadas en la esquina hasta que se llenen. ¿Cuántas se van a comer? Depende del hambre, ¿cierto?</li>
      <li>Buscar wifi en el celular hasta que se conecte.</li>
    </ul>
    <div class="codigo">
      <div class="codigo-titulo">¿Cómo se ve esto en C#?</div>
      <pre><code>{`int dinero = 50000;
int precioEmpanada = 2000;
while (dinero >= precioEmpanada) {
    Console.WriteLine("¡Puedo comprar una empanada!");
    dinero -= precioEmpanada;
}`}</code></pre>
    </div>
    <div class="alerta">
      <b>⚠️ ¡Cuidado con los ciclos infinitos!</b> Siempre asegúrate de que la condición cambie dentro del ciclo, si no, ¡el programa se queda pegado!
    </div>
  </section>

  <section class="arreglos-section">
    <h2>🧺 ¿Qué Son los Arreglos? - Tu Colección de Tazos, Pero en el Computador</h2>
    <p>Un <b>arreglo</b> es como una cajita con varios compartimentos, donde cada compartimento guarda un dato. ¡Pero ojo! Usualmente, todos los datos en un arreglo son del mismo tipo (todos números, o todas palabras, etc.).</p>
    <ul>
      <li>Una <b>lista de convocados</b> para el partido del Nacional o del Medellín.</li>
      <li>Su <b>playlist de Spotify</b> con sus canciones favoritas.</li>
      <li>Una <b>cartuchera</b> donde guardan lapiceros de varios colores.</li>
      <li>Los <b>ingredientes</b> para una arepa: harina, agua, sal, quesito...</li>
    </ul>
    <div class="codigo">
      <div class="codigo-titulo">¿Cómo creamos y usamos arreglos en C#?</div>
      <pre><code>{`string[] parchesEnMedellin = {"Ir al Parque Lleras", "Subir al Pueblito Paisa", "Caminar por la 70", "Visitar Guatapé", "Comer en el Mercado del Río"};
Console.WriteLine("El primer parche es: " + parchesEnMedellin[0]);
Console.WriteLine("Tengo " + parchesEnMedellin.Length + " parches planeados.");`}</code></pre>
    </div>
  </section>

  <section class="ciclos-arreglos">
    <h2>🤝 Ciclos y Arreglos Juntos: ¡La Combinación Ganadora!</h2>
    <p>Si tienen una lista de 100 amigos en un arreglo, ¿van a escribir 100 líneas de código para saludarlos uno por uno? ¡Ni locos! Usamos un ciclo.</p>
    <div class="codigo">
      <div class="codigo-titulo">Recorriendo un arreglo con <code>for</code>:</div>
      <pre><code>{`for (int i = 0; i < parchesEnMedellin.Length; i++) {
    Console.WriteLine("Parche #" + (i + 1) + ": " + parchesEnMedellin[i]);
}`}</code></pre>
    </div>
    <div class="codigo">
      <div class="codigo-titulo">Recorriendo un arreglo con <code>foreach</code>:</div>
      <pre><code>{`foreach (string comida in comidasTipicasDeAntioquia) {
    Console.WriteLine("¡Qué rico sería comer: " + comida + "!");
}`}</code></pre>
    </div>
  </section>

  <section class="ejercicios-section">
    <h2>🛠️ ¡A "Echar Código"! Ejercicios Bien Paisas</h2>
    <ol>
      <li><b>Lista de Tareas del Finde:</b> Crea un arreglo llamado <code>tareasDelFinde</code> con 5 tareas que suelan hacer un fin de semana en Medellín. Usa un ciclo <code>for</code> para imprimir cada tarea diciendo: "Este finde tengo que: [nombre de la tarea]".</li>
      <li><b>Ahorrando pa' las Boletas:</b> Imagina que quieres ahorrar para las boletas de un concierto de tu artista favorito, que valen $150.000. Empiezas con $0 ahorrados. Cada "semana" ahorras $20.000. Usa un ciclo <code>while</code> para simular cuántas semanas necesitas ahorrar hasta que tengas suficiente para las boletas. Muestra cuánto llevas ahorrado cada semana.</li>
      <li><b>Ídolos del Fútbol Paisa:</b> Crea un arreglo llamado <code>idolosDelFutbol</code> con 3 de tus jugadores favoritos del Nacional o del Medellín. Usa un ciclo <code>foreach</code> para imprimir el nombre de cada jugador con un mensaje emotivo.</li>
      <li><b>Ingredientes pa' la Arepa:</b> Crea un arreglo llamado <code>ingredientesArepa</code> con los ingredientes básicos para hacer una arepa paisa. Usa un ciclo <code>for</code> o <code>foreach</code> para mostrar cada ingrediente.</li>
      <li><b>Desafío: La Tiendita de la Esquina:</b> Crea dos arreglos: <code>productosTienda</code> (string): {"Gaseosa", "Papitas", "Chocolatina", "Buñuelo"} y <code>preciosTienda</code> (int): {2500, 1800, 1200, 1500}. Simula una compra preguntando al usuario qué producto quiere comprar y suma el total usando un ciclo <code>while</code>.</li>
    </ol>
  </section>

  <section class="resumen-section">
    <h2>📝 Pa' que no se te Olvide, Parse - Resumen y Consejos</h2>
    <ul>
      <li><b>Ciclos <code>for</code>:</b> Cuando sabés cuántas veces. (Inicio, condición, incremento).</li>
      <li><b>Ciclos <code>while</code>:</b> Mientras una condición sea verdad. (¡Cuidado con los infinitos!).</li>
      <li><b>Arreglos (Arrays):</b> Cajitas para guardar listas de datos del mismo tipo. ¡Los índices empiezan en 0!</li>
      <li><b><code>foreach</code>:</b> Forma fácil de recorrer todos los elementos de un arreglo.</li>
    </ul>
    <div class="consejos">
      <b>Consejos de un Parcero Programador:</b>
      <ul>
        <li>¡Practicá, practicá, practicá! "Echar código" es la única forma de volverse un teso.</li>
        <li>No te dé pena preguntar. Si te enredás, ¡preguntá! A tus profes, a tus compañeros, en internet.</li>
        <li>Usá <code>Console.WriteLine()</code> como tu mejor amigo. Pa' ver qué está pasando en tu código.</li>
        <li>Leé código de otros. Cuando veas ejemplos, trata de entender cómo funcionan.</li>
        <li>¡Conectate con la comunidad! En Medellín hay gente muy pila en esto:
          <ul>
            <li><b>MedellinJS</b> (Aunque es de JavaScript, se aprende mucho de lógica de programación)</li>
            <li><b>.NET Medellín</b> (¡Perfecto para los que le están dando al C#!)</li>
            <li><b>Ruta N</b> (Siempre tienen eventos y charlas bacanas de tecnología)</li>
          </ul>
        </li>
      </ul>
    </div>
  </section>

  <section class="final-section">
    <h2>🎉 ¡A Programar se Dijo, Pues!</h2>
    <p>¡Listo, futuro crack de la programación! Ya tenés las bases de los ciclos y arreglos. Ahora te toca a vos experimentar, crear cosas chéveres y, sobre todo, ¡divertirte aprendiendo!</p>
    <p>Si tenés preguntas o querés mostrar lo que hiciste, ¡no dudes en compartirlo!</p>
    <div class="exito">¡Éxitos en tu camino como programador/a paisa! 🇨🇴👨‍💻👩‍💻</div>
  </section>

  <section class="extra-ejemplo">
    <h3>🔽 Ciclo <code>for</code> descendente: Contando hacia atrás</h3>
    <p>¿Y si queremos hacer una cuenta regresiva, como cuando va a empezar el partido en el Atanasio?</p>
    <div class="codigo">
      <div class="codigo-titulo">Cuenta regresiva con <code>for</code>:</div>
      <pre><code>{`for (int i = 5; i >= 1; i--) {
    Console.WriteLine("Faltan " + i + " segundos para el inicio!");
}
Console.WriteLine("¡Arrancó el partido!");`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`Faltan 5 segundos para el inicio!
Faltan 4 segundos para el inicio!
Faltan 3 segundos para el inicio!
Faltan 2 segundos para el inicio!
Faltan 1 segundos para el inicio!
¡Arrancó el partido!`}</code></pre>
    </div>
  </section>

  <section class="extra-ejemplo">
    <h3>📊 Promedio de Notas con Arreglos y Ciclo <code>for</code></h3>
    <p>Supongamos que tienes las notas de tus 4 materias favoritas y quieres saber tu promedio:</p>
    <div class="codigo">
      <div class="codigo-titulo">Cálculo del promedio:</div>
      <pre><code>{`int[] notas = {4, 5, 3, 4};
int suma = 0;
for (int i = 0; i < notas.Length; i++) {
    suma += notas[i];
}
double promedio = (double)suma / notas.Length;
Console.WriteLine("Tu promedio es: " + promedio);`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`Tu promedio es: 4`}</code></pre>
    </div>
  </section>

  <section class="enlace-ejercicios38">
    <a href="/decimo/algoritmos/ciclosyarreglos/ejercicios38" class="btn-ejercicios38">
      📚 Ver los 38 ejercicios propuestos para practicar (quiz)
    </a>
  </section>

  <section class="enlace-funciones">
    <a href="/decimo/algoritmos/funciones" class="btn-funciones">
      🧑‍💻 Aprende todo sobre funciones en C# (explicación y ejercicios)
    </a>
  </section>
</main>

<style>
.clase2-container {
  max-width: 800px;
  margin: 2rem auto;
  padding: 2rem;
  background: #fff;
  border-radius: 1.5rem;
  box-shadow: 0 4px 24px 0 #0002;
  font-family: 'Segoe UI', Arial, sans-serif;
}
.intro h1 {
  color: #0e7490;
  font-size: 2.2rem;
  margin-bottom: 0.5rem;
}
.bienvenida {
  font-size: 1.1rem;
  margin-bottom: 1rem;
}
.destacado {
  background: #e0f2fe;
  border-left: 5px solid #0ea5e9;
  padding: 0.7rem 1rem;
  margin: 1rem 0;
  font-weight: bold;
  border-radius: 0.5rem;
}
.frase {
  color: #0ea5e9;
  font-weight: bold;
}
section {
  margin-bottom: 2.5rem;
}
h2, h3 {
  color: #0e7490;
  margin-bottom: 0.5rem;
}
.codigo {
  background: #f1f5f9;
  border-radius: 0.5rem;
  padding: 1rem;
  margin: 1rem 0;
  font-size: 1rem;
  overflow-x: auto;
}
.codigo-titulo {
  font-weight: bold;
  margin-bottom: 0.3rem;
}
.codigo-resultado {
  color: #059669;
  font-weight: bold;
  margin-top: 0.7rem;
}
.ejemplo-paisa {
  background: #fef9c3;
  border-left: 5px solid #facc15;
  padding: 0.7rem 1rem;
  margin: 1rem 0;
  border-radius: 0.5rem;
}
.codigo-responsive {
  background: #fef9c3;
  border-radius: 0.5rem;
  padding: 0.5rem 0.3rem 0.5rem 0.7rem;
  margin: 0.7rem 0 0.5rem 0;
  overflow-x: auto;
  font-size: 0.97rem;
  max-width: 100%;
}
.codigo-responsive pre {
  margin: 0;
  white-space: pre-wrap;
  word-break: break-all;
}
.alerta {
  background: #fee2e2;
  color: #b91c1c;
  border-left: 5px solid #ef4444;
  padding: 0.7rem 1rem;
  margin: 1rem 0;
  border-radius: 0.5rem;
  font-weight: bold;
}
.ejercicios-section ol {
  margin-left: 1.5rem;
}
.ejercicios-section li {
  margin-bottom: 0.7rem;
}
.resumen-section ul {
  margin-left: 1.5rem;
}
.consejos ul {
  margin-left: 1.5rem;
}
.final-section {
  text-align: center;
  background: #e0f2fe;
  border-radius: 1rem;
  padding: 1.5rem 1rem 1rem 1rem;
  margin-top: 2rem;
}
.exito {
  color: #059669;
  font-size: 1.2rem;
  font-weight: bold;
  margin-top: 1rem;
}
.extra-ejemplo {
  background: #f0fdf4;
  border-left: 5px solid #22c55e;
  border-radius: 0.5rem;
  padding: 1rem 1.2rem;
  margin: 1.5rem 0;
}
.enlace-ejercicios38 {
  text-align: center;
  margin: 2.5rem 0 1.5rem 0;
}
.btn-ejercicios38 {
  display: inline-block;
  background: #0ea5e9;
  color: #fff;
  font-weight: bold;
  font-size: 1.1rem;
  padding: 0.8rem 1.5rem;
  border-radius: 0.7rem;
  text-decoration: none;
  box-shadow: 0 2px 8px #0001;
  transition: background 0.2s;
}
.btn-ejercicios38:hover {
  background: #0369a1;
}
.enlace-funciones {
  text-align: center;
  margin: 2.5rem 0 1.5rem 0;
}
.btn-funciones {
  display: inline-block;
  background: #059669;
  color: #fff;
  font-weight: bold;
  font-size: 1.1rem;
  padding: 0.8rem 1.5rem;
  border-radius: 0.7rem;
  text-decoration: none;
  box-shadow: 0 2px 8px #0001;
  transition: background 0.2s;
}
.btn-funciones:hover {
  background: #047857;
}
@media (max-width: 600px) {
  .clase2-container {
    padding: 0.7rem 0.2rem;
    margin: 0.5rem auto;
    border-radius: 0.7rem;
  }
  .intro h1 {
    font-size: 1.3rem;
  }
  .codigo-responsive {
    font-size: 0.85rem;
    padding: 0.4rem 0.05rem 0.4rem 0.2rem;
  }
}
</style>
