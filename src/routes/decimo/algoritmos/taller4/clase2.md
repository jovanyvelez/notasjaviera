# 24 Ejercicios de Switch en C# 

## Ejercicios Básicos (1-8)

### 1. Días de la Semana
Escribe un programa que reciba un número del 1 al 7 y muestre el día de la semana correspondiente.
**Tip:** Usa `int dia` como variable y cada `case` para un número del 1-7.

### 2. Calificaciones con Letras
Crea un programa que convierta calificaciones numéricas (1-5) a letras (A, B, C, D, F).
**Tip:** 5=A, 4=B, 3=C, 2=D, 1=F. No olvides el `default` para valores inválidos.

### 3. Meses del Año
Desarrolla un programa que muestre el nombre del mes según un número del 1 al 12.
**Tip:** Enero=1, Febrero=2, etc. Usa `default` para mostrar "Mes inválido".

### 4. Operaciones Matemáticas Básicas
Haz un programa que reciba dos números y un operador (+, -, *, /) y realice la operación.
**Tip:** Usa `char operador` y cada `case` para un símbolo matemático.

### 5. Colores del Semáforo
Programa que reciba un color (rojo, amarillo, verde) y muestre la acción correspondiente.
**Tip:** Usa `string color` y recuerda usar `.ToLower()` para evitar problemas de mayúsculas.

### 6. Estaciones del Año
Crea un programa que determine la estación según el número de mes ingresado.
**Tip:** Agrupa los meses: 12,1,2=Invierno, 3,4,5=Primavera, etc.

### 7. Figuras Geométricas
Programa que calcule el área de diferentes figuras según la opción elegida (1=cuadrado, 2=círculo, 3=triángulo).
**Tip:** Para cada `case`, pide los datos necesarios y usa las fórmulas correspondientes.

### 8. Conversión de Unidades
Desarrolla un conversor de temperatura que permita elegir entre Celsius a Fahrenheit o viceversa.
**Tip:** Usa números para las opciones (1=C a F, 2=F a C) y las fórmulas de conversión.

## Ejercicios Intermedios (9-16)

### 9. Calculadora de IMC por Categorías
Programa que calcule el IMC y use `switch` para mostrar la categoría (bajo peso, normal, sobrepeso, obesidad).
**Tip:** Calcula el IMC primero y luego usa rangos con `switch` sobre valores enteros.

### 10. Juego de Piedra, Papel o Tijera
Crea un juego donde el usuario y la computadora eligen, y determina el ganador.
**Tip:** Usa números (1=piedra, 2=papel, 3=tijera) y combina las opciones del usuario y la PC.

### 11. **Ejercicio: Sistema de Pedido Simple**

## Enunciado
Crea un programa que simule un pedido en una cafetería. El usuario puede elegir **máximo 3 productos** de un menú y el programa debe calcular el total a pagar.

### Menú:
- Café - $2.50
- Sandwich - $4.75
- Galletas - $1.25
- Jugo - $3.00
- Muffin - $2.80

### Requisitos:
1. Muestra el menú al usuario
2. Pide que seleccione su **primer producto** (número del 1 al 5)
3. Pide que seleccione su **segundo producto** (número del 1 al 5, o 0 si no quiere más)
4. Pide que seleccione su **tercer producto** (número del 1 al 5, o 0 si no quiere más)
5. Calcula y muestra el total a pagar
6. Muestra un resumen de lo que pidió

### Ejemplo de ejecución:
```
=== CAFETERÍA LA ESQUINA ===
1. Café - $2.50
2. Sandwich - $4.75
3. Galletas - $1.25
4. Jugo - $3.00
5. Muffin - $2.80

Seleccione su primer producto (1-5): 2
¡Sandwich agregado!

Seleccione su segundo producto (1-5, o 0 para terminar): 1
¡Café agregado!

Seleccione su tercer producto (1-5, o 0 para terminar): 0

=== RESUMEN DE SU PEDIDO ===
- Sandwich: $4.75
- Café: $2.50
TOTAL A PAGAR: $7.25
```

## Pistas para la solución:
- Usa **if-else if** en lugar de switch para manejar las opciones
- Usa una variable `double total = 0` para acumular los precios
- Usa variables `string` para recordar qué pidió el usuario (ej: `producto1`, `producto2`, `producto3`)
- Para cada selección, verifica si es 0 (no quiere más productos) antes de procesar
- Al final, usa **if** para mostrar solo los productos que realmente pidió (que no sean vacíos)

## Desafío adicional:
Agrega validación para que si el usuario ingresa un número inválido (menor que 0 o mayor que 5), muestre un mensaje de error y no agregue nada al pedido.

### 12. Clasificador de Edades
Clasifica personas según su edad en categorías (niño, adolescente, adulto, adulto mayor).
**Tip:** Divide la edad entre 10 y usa el resultado en el `switch` para agrupar rangos.

### 13. Días Laborables vs Fin de Semana
Programa que determine si un día es laboral o fin de semana según el número ingresado.
**Tip:** Agrupa los casos: 1-5 para días laborables, 6-7 para fin de semana.

### 14. Conversor de Notas Musicales
Convierte números (1-7) a notas musicales (Do, Re, Mi, Fa, Sol, La, Si).
**Tip:** Directo: 1=Do, 2=Re, etc. Considera agregar sostenidos como casos extra.

### 15. Sistema de Descuentos
Programa que aplique descuentos según el tipo de cliente (estudiante, adulto mayor, empleado).
**Tip:** Usa `string` para el tipo de cliente y calcula el descuento correspondiente.

### 16. Planetas del Sistema Solar
Muestra información sobre planetas según la posición desde el Sol (1=Mercurio, 2=Venus, etc.).
**Tip:** Cada `case` puede mostrar datos como distancia, tamaño o características.

## Ejercicios Avanzados (17-24)

### 17. Calculadora Científica Básica
Extiende la calculadora básica con operaciones como potencia, raíz cuadrada y porcentaje.
**Tip:** Usa `char` o `string` para operadores especiales como "^", "sqrt", "%".

### 18. Conversor de Bases Numéricas
Programa que convierta números entre decimal, binario y hexadecimal.
**Tip:** Usa `Convert.ToString(numero, base)` y `Convert.ToInt32(texto, base)`.

### 19. Simulador de Cajero Automático
Crea un menú de cajero con opciones como consultar saldo, retirar, depositar.
**Tip:** Usa una variable `saldo` que se modifique según la opción elegida.

### 20. Clasificador de Triángulos
Programa que determine el tipo de triángulo según sus lados (equilátero, isósceles, escaleno).
**Tip:** Cuenta cuántos lados son iguales y usa ese número en el `switch`.

### 21. Generador de Contraseñas por Nivel
Crea contraseñas según el nivel de seguridad elegido (básico, medio, alto).
**Tip:** Cada nivel puede tener diferente longitud y tipos de caracteres.

### 22. Sistema de Calificación Deportiva
Programa que califique el rendimiento en un deporte según puntos obtenidos.
**Tip:** Divide los puntos en rangos y usa división entera para el `switch`.

### 23. Conversor de Tiempo
Convierte tiempo entre diferentes unidades (segundos, minutos, horas, días).
**Tip:** Usa el menú para elegir conversión y aplica los factores correspondientes.

### 24. Simulador de Juego de Dados
Simula el lanzamiento de dados y determina combinaciones especiales (par, escalera, etc.).
**Tip:** Suma los dados o analiza patrones, luego usa `switch` para los resultados especiales.

## Consejos Generales para Todos los Ejercicios:

1. **Siempre incluye `default`:** Para manejar casos no válidos
2. **Usa `break`:** No olvides terminar cada caso
3. **Valida la entrada:** Verifica que los datos sean correctos
4. **Agrupa casos similares:** Puedes usar múltiples `case` sin `break` entre ellos
5. **Considera mayúsculas/minúsculas:** Usa `.ToLower()` o `.ToUpper()` con strings
6. **Documenta tu código:** Agrega comentarios para explicar la lógica

¡Estos ejercicios te ayudarán a dominar la instrucción `switch` en C#!