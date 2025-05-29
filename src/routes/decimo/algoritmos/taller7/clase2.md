# Ciclos For y Arrays en C# Moderno (.NET 9)

¡Hola programadores! Hoy vamos a explorar dos conceptos fundamentales que van de la mano en C#: los ciclos `for` y los arrays (arreglos). Estos son herramientas esenciales que te permitirán manejar colecciones de datos y automatizar tareas repetitivas.

## ¿Qué son los Arrays?

Un **array** es como una caja con múltiples compartimentos numerados donde puedes almacenar varios elementos del mismo tipo. Imagina una estantería con libros: cada libro ocupa una posición específica y puedes acceder a cualquier libro sabiendo su posición.

### Sintaxis Básica de Arrays

```csharp
// Declaración y inicialización
int[] numeros = new int[5];  // Array de 5 enteros
string[] nombres = {"Ana", "Luis", "María", "Carlos"};  // Array inicializado con valores
double[] precios = new double[] {10.5, 25.0, 15.75};  // Otra forma de inicializar
```

### Características Importantes de los Arrays

- **Índice base cero**: El primer elemento está en la posición 0
- **Tamaño fijo**: Una vez creado, no puedes cambiar su tamaño
- **Tipo homogéneo**: Todos los elementos deben ser del mismo tipo
- **Acceso directo**: Puedes ir directamente a cualquier posición

```csharp
string[] frutas = {"manzana", "banana", "naranja", "uva"};

// Acceso a elementos
Console.WriteLine(frutas[0]);  // "manzana"
Console.WriteLine(frutas[3]);  // "uva"

// Modificación de elementos
frutas[1] = "pera";  // Cambia "banana" por "pera"

// Propiedad Length para obtener el tamaño
Console.WriteLine($"El array tiene {frutas.Length} elementos");
```

## El Ciclo For: Tu Mejor Aliado

El ciclo `for` es perfecto para recorrer arrays porque sabes exactamente cuántas veces necesitas repetir una acción. Es como tener un contador automático que te ayuda a visitar cada compartimento de tu estantería.

### Estructura del Ciclo For

```csharp
for (inicialización; condición; incremento)
{
    // Código a ejecutar en cada iteración
}
```

### Ejemplo Básico

```csharp
// Mostrar números del 1 al 5
for (int i = 1; i <= 5; i++)
{
    Console.WriteLine($"Número: {i}");
}
```

**Explicación paso a paso:**
1. `int i = 1`: Inicializa la variable contador en 1
2. `i <= 5`: Mientras i sea menor o igual a 5, continúa el ciclo
3. `i++`: Después de cada iteración, incrementa i en 1

## Combinando For y Arrays: La Dupla Perfecta

### Recorriendo un Array con For

```csharp
int[] calificaciones = {85, 92, 78, 96, 88};

// Mostrar todas las calificaciones
for (int i = 0; i < calificaciones.Length; i++)
{
    Console.WriteLine($"Calificación {i + 1}: {calificaciones[i]}");
}
```

**¿Por qué `i < calificaciones.Length`?**
- Los arrays empiezan en índice 0
- Si el array tiene 5 elementos, los índices van de 0 a 4
- `Length` devuelve 5, por eso usamos `<` en lugar de `<=`

### Ejemplos Prácticos

#### 1. Calculando el Promedio

```csharp
double[] notas = {8.5, 9.2, 7.8, 9.6, 8.8};
double suma = 0;

// Sumar todas las notas
for (int i = 0; i < notas.Length; i++)
{
    suma += notas[i];
}

double promedio = suma / notas.Length;
Console.WriteLine($"El promedio es: {promedio:F2}");
```

#### 2. Encontrar el Valor Máximo

```csharp
int[] temperaturas = {22, 28, 19, 31, 25, 18, 29};
int maxima = temperaturas[0];  // Asumimos que el primero es el mayor

for (int i = 1; i < temperaturas.Length; i++)
{
    if (temperaturas[i] > maxima)
    {
        maxima = temperaturas[i];
    }
}

Console.WriteLine($"La temperatura máxima fue: {maxima}°C");
```

#### 3. Contando Elementos que Cumplen una Condición

```csharp
int[] edades = {15, 22, 17, 19, 16, 25, 14};
int menoresDeEdad = 0;

for (int i = 0; i < edades.Length; i++)
{
    if (edades[i] < 18)
    {
        menoresDeEdad++;
    }
}

Console.WriteLine($"Hay {menoresDeEdad} menores de edad");
```

## Características Modernas de C# (.NET 9)

### 1. Inicialización con `new[]`

```csharp
// El compilador infiere el tipo automáticamente
var colores = new[] {"rojo", "verde", "azul", "amarillo"};
var numeros = new[] {1, 2, 3, 4, 5};
```

### 2. Índices y Rangos

```csharp
string[] animales = {"perro", "gato", "pájaro", "pez", "hamster"};

// Acceso desde el final con ^
Console.WriteLine(animales[^1]);  // "hamster" (último elemento)
Console.WriteLine(animales[^2]);  // "pez" (penúltimo elemento)

// Rangos con ..
string[] primerosTres = animales[0..3];  // {"perro", "gato", "pájaro"}
string[] ultimosDos = animales[^2..];    // {"pez", "hamster"}
```

### 3. Foreach: Una Alternativa Elegante

Cuando solo necesitas leer los elementos (no modificar ni usar el índice):

```csharp
string[] ciudades = {"Medellín", "Bogotá", "Cali", "Cartagena"};

// Con for tradicional
for (int i = 0; i < ciudades.Length; i++)
{
    Console.WriteLine(ciudades[i]);
}

// Con foreach (más limpio para solo lectura)
foreach (string ciudad in ciudades)
{
    Console.WriteLine(ciudad);
}
```

## Variaciones del Ciclo For

### For con Incremento Diferente

```csharp
// Números pares del 0 al 10
for (int i = 0; i <= 10; i += 2)
{
    Console.WriteLine(i);
}

// Conteo regresivo
for (int i = 10; i >= 1; i--)
{
    Console.WriteLine($"Faltan {i} segundos...");
}
```

### For con Múltiples Variables

```csharp
int[] array1 = {1, 2, 3, 4, 5};
int[] array2 = {10, 20, 30, 40, 50};

// Recorrer dos arrays simultáneamente
for (int i = 0, j = array2.Length - 1; i < array1.Length; i++, j--)
{
    Console.WriteLine($"{array1[i]} + {array2[j]} = {array1[i] + array2[j]}");
}
```

## Errores Comunes y Cómo Evitarlos

### 1. Índice Fuera de Rango

```csharp
int[] numeros = {1, 2, 3};

// ❌ ERROR: Índice fuera de rango
// for (int i = 0; i <= numeros.Length; i++)

// ✅ CORRECTO
for (int i = 0; i < numeros.Length; i++)
{
    Console.WriteLine(numeros[i]);
}
```

### 2. Modificar el Array Durante el Recorrido

```csharp
List<int> lista = new List<int> {1, 2, 3, 4, 5};

// ❌ PROBLEMÁTICO: Modificar la colección mientras la recorres
// foreach (int numero in lista)
// {
//     if (numero % 2 == 0)
//         lista.Remove(numero);  // Esto puede causar errores
// }

// ✅ CORRECTO: Usar for descendente para eliminaciones
for (int i = lista.Count - 1; i >= 0; i--)
{
    if (lista[i] % 2 == 0)
        lista.RemoveAt(i);
}
```

## Ejercicios Prácticos

### Ejercicio 1: Gestión de Inventario
Crea un programa que maneje el inventario de una tienda:

```csharp
string[] productos = {"Laptop", "Mouse", "Teclado", "Monitor", "Audífonos"};
int[] cantidades = {5, 15, 8, 3, 12};
double[] precios = {1200.0, 25.0, 75.0, 300.0, 50.0};

// Tu tarea: Calcular el valor total del inventario
// Mostrar productos con stock bajo (menos de 5 unidades)
// Encontrar el producto más caro
```

### Ejercicio 2: Análisis de Ventas
```csharp
double[] ventasSemanales = {1500.50, 2300.75, 1800.25, 2100.00, 1950.80, 2800.90, 1650.45};

// Tu tarea: Calcular promedio de ventas
// Encontrar el día con mayores y menores ventas
// Contar cuántos días superaron el promedio
```

## Consejos Pro

1. **Usa nombres descriptivos**: `for (int indice = 0; ...)` es mejor que `for (int i = 0; ...)`
2. **Evita números mágicos**: Usa `array.Length` en lugar de números fijos
3. **Considera foreach**: Para lectura simple, `foreach` es más legible
4. **Valida los datos**: Siempre verifica que el array no esté vacío antes de procesarlo
5. **Usa var con cuidado**: Solo cuando el tipo sea obvio del contexto

## Resumen

Los ciclos `for` y los arrays son herramientas poderosas que trabajan juntas para:
- Almacenar colecciones de datos relacionados
- Procesar información de manera eficiente
- Automatizar tareas repetitivas
- Realizar cálculos sobre conjuntos de datos

Dominar estos conceptos te dará una base sólida para abordar problemas más complejos en programación. La práctica constante es clave: mientras más experimentes con diferentes combinaciones, más natural se volverá su uso.

¡Ahora es tu turno de practicar! Crea tus propios arrays y experimenta con diferentes tipos de ciclos for. Recuerda que cada error es una oportunidad de aprendizaje.