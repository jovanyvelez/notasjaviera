<script>
// Componente educativo, solo visual
</script>

<main class="funciones-cs-container">
  <section class="intro">
    <h1>🧑‍🏫 Funciones en C# — ¡El Secreto de los Programadores Tesos!</h1>
    <p class="bienvenida">¡Hola parceros y parceras! Hoy vamos a aprender sobre <b>funciones</b> en C#, una de las herramientas más poderosas para que tu código sea organizado, fácil de entender y reutilizable. Imagina que eres un chef y tienes recetas para todo: cada receta es una función que puedes usar cuando la necesites. ¡Así funciona en programación!</p>
  </section>

  <section class="que-es">
    <h2>¿Qué es una función?</h2>
    <p>Una función es un bloque de código que realiza una tarea específica. Puedes llamarla (usarla) las veces que quieras, sin tener que escribir el mismo código una y otra vez. Es como tener un "truco" guardado para cuando lo necesites.</p>
    <ul>
      <li>Te ayuda a <b>organizar</b> tu código.</li>
      <li>Evita repetir lo mismo muchas veces.</li>
      <li>Hace que tu programa sea más fácil de leer y mantener.</li>
    </ul>
  </section>

  <section class="ejemplo-basico">
    <h2>Ejemplo básico: Una función que saluda</h2>
    <div class="codigo">
      <div class="codigo-titulo">Definición y uso de una función:</div>
      <pre><code>{`void Saludar() {
    Console.WriteLine("¡Hola, bienvenido a la clase de C#!");
}

// Para usarla (llamarla):
Saludar();`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`¡Hola, bienvenido a la clase de C#!`}</code></pre>
    </div>
    <p><b>¿Ves? Solo defines la función una vez y la puedes usar todas las veces que quieras.</b></p>
  </section>

  <section class="parametros">
    <h2>Funciones con parámetros: ¡Personaliza tu receta!</h2>
    <p>Un parámetro es como un ingrediente que le pasas a la función para que haga algo diferente según lo que le des.</p>
    <div class="codigo">
      <div class="codigo-titulo">Función con parámetro:</div>
      <pre><code>{`void SaludarA(string nombre) {
    Console.WriteLine("¡Hola, " + nombre + "!");
}

SaludarA("Sofía");
SaludarA("Juan");`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`¡Hola, Sofía!
¡Hola, Juan!`}</code></pre>
    </div>
  </section>

  <section class="retorno">
    <h2>Funciones que devuelven un valor</h2>
    <p>Algunas funciones no solo hacen algo, sino que también <b>devuelven</b> un resultado. Por ejemplo, una función que suma dos números y te da el resultado.</p>
    <div class="codigo">
      <div class="codigo-titulo">Función que retorna un valor:</div>
      <pre><code>{`int Sumar(int a, int b) {
    return a + b;
}

int resultado = Sumar(7, 5);
Console.WriteLine("La suma es: " + resultado);`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`La suma es: 12`}</code></pre>
    </div>
  </section>

  <section class="explicacion">
    <h2>¿Cómo se estructura una función en C#?</h2>
    <ul>
      <li><b>Tipo de retorno</b>: ¿Qué devuelve la función? (Ej: <code>void</code> si no devuelve nada, <code>int</code> si devuelve un número entero, <code>string</code> si devuelve texto, etc.)</li>
      <li><b>Nombre</b>: El nombre de la función (¡ponle nombres claros!).</li>
      <li><b>Parámetros</b>: Los datos que recibe la función (pueden ser cero, uno o varios).</li>
      <li><b>Cuerpo</b>: El bloque de código entre llaves <code>&#123; &#125;</code> que hace el trabajo.</li>
    </ul>
    <div class="codigo">
      <div class="codigo-titulo">Ejemplo general:</div>
      <pre><code>{`tipoDeRetorno NombreFuncion(parámetros) {
    // Código que realiza la tarea
    return valor; // (si no es void)
}`}</code></pre>
    </div>
  </section>

  <section class="ejemplos-extra">
    <h2>Ejemplos prácticos para la vida real</h2>
    <div class="codigo">
      <div class="codigo-titulo">Función para calcular el promedio de 3 notas:</div>
      <pre><code>{`double Promedio(double n1, double n2, double n3) {
    return (n1 + n2 + n3) / 3;
}

Console.WriteLine("El promedio es: " + Promedio(4.5, 3.8, 5));`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`El promedio es: 4.433333333333334`}</code></pre>
    </div>
    <div class="codigo">
      <div class="codigo-titulo">Función para saber si un número es par:</div>
      <pre><code>{`bool EsPar(int numero) {
    return numero % 2 == 0;
}

Console.WriteLine(EsPar(8)); // true
Console.WriteLine(EsPar(7)); // false`}</code></pre>
      <div class="codigo-resultado">Resultado en la consola:</div>
      <pre><code>{`True
False`}</code></pre>
    </div>
  </section>

  <section class="consejos">
    <h2>Consejos de profe para que seas un teso con funciones</h2>
    <ul>
      <li>¡Ponle nombres claros a tus funciones! Así sabrás para qué sirve cada una.</li>
      <li>Si una tarea se repite, ¡haz una función!</li>
      <li>Practica creando funciones con y sin parámetros, y que devuelvan o no valores.</li>
      <li>Lee código de otros y trata de entender cómo usan funciones.</li>
      <li>No te dé miedo experimentar: ¡prueba, equivócate y aprende!</li>
    </ul>
  </section>

  <section class="ejercicios">
    <h2>🛠️ Ejercicios propuestos</h2>
    <ol>
      <li>Crea una función que reciba un nombre y salude a esa persona.</li>
      <li>Haz una función que reciba dos números y devuelva su producto.</li>
      <li>Escribe una función que reciba una edad y diga si es mayor o menor de edad.</li>
      <li>Crea una función que reciba un arreglo de enteros y devuelva la suma total.</li>
      <li>Haz una función que reciba una nota y devuelva "Aprobado" si es mayor o igual a 3, o "Reprobado" si es menor.</li>
      <li>Escribe una función que reciba un número y devuelva su cuadrado.</li>
      <li>Crea una función que reciba un arreglo de nombres y los imprima uno por uno.</li>
      <li>Haz una función que reciba un número y devuelva true si es múltiplo de 5.</li>
      <li>Escribe una función que reciba dos textos y los una en uno solo.</li>
      <li>Crea una función que reciba una lista de notas y devuelva el promedio.</li>
    </ol>
  </section>
</main>

<style>
.funciones-cs-container {
  max-width: 800px;
  margin: 2rem auto;
  padding: 2rem 1rem;
  background: #f8fafc;
  border-radius: 1.5rem;
  box-shadow: 0 4px 24px 0 #0001;
  font-family: 'Segoe UI', Arial, sans-serif;
}
.funciones-cs-container h1 {
  color: #0e7490;
  font-size: 2rem;
  margin-bottom: 1rem;
  text-align: center;
}
.funciones-cs-container .bienvenida {
  font-size: 1.1rem;
  margin-bottom: 1.5rem;
  text-align: center;
}
section {
  margin-bottom: 2.2rem;
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
.ejercicios ol {
  margin-left: 1.5rem;
  font-size: 1.05rem;
}
.ejercicios li {
  margin-bottom: 0.7rem;
  background: #e0f2fe;
  border-left: 5px solid #0ea5e9;
  border-radius: 0.5rem;
  padding: 0.7rem 1rem;
  list-style-position: inside;
}
@media (max-width: 600px) {
  .funciones-cs-container {
    padding: 0.7rem 0.1rem;
    border-radius: 0.7rem;
  }
  .funciones-cs-container h1 {
    font-size: 1.2rem;
  }
  .ejercicios ol {
    font-size: 0.97rem;
  }
}
</style>
