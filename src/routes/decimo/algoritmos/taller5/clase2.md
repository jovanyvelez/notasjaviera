# 24 Ejercicios de Operadores Lógicos && y || en C#

## Ejercicios Básicos (1-8)

### 1. Verificar si un número está en un rango
Escribe un programa que lea un número entero y verifique si está entre 1 y 100 (inclusive).
**Pista:** Usa `numero >= 1 && numero <= 100`


### 2. Validar usuario y contraseña
Crea un programa que verifique si el usuario es "admin" Y la contraseña es "123456".
**Pista:** Usa `usuario == "admin" && contraseña == "123456"`

### 3. Verificar si es fin de semana
Escribe un programa que lea un día de la semana (como número: 1=lunes, 7=domingo) y determine si es fin de semana.
**Pista:** Fin de semana es sábado (6) O domingo (7): `dia == 6 || dia == 7`

### 4. Comprobar si puede votar
Crea un programa que determine si una persona puede votar (mayor o igual a 18 años Y ciudadano).
**Pista:** Usa dos variables booleanas y el operador &&

### 5. Verificar números pares en un rango
Escribe un programa que verifique si un número es par Y está entre 10 y 50.
**Pista:** Para par usa `numero % 2 == 0`, luego combina con &&

### 6. Validar nota aprobatoria
Crea un programa que determine si un estudiante aprueba (nota >= 6) O tiene una segunda oportunidad (nota >= 4).
**Pista:** Usa `nota >= 6 || nota >= 4` para mostrar diferentes mensajes

### 7. Verificar año bisiesto simple
Escribe un programa que determine si un año es divisible por 4 Y no es divisible por 100.
**Pista:** `año % 4 == 0 && año % 100 != 0`

### 8. Comprobar caracteres válidos
Crea un programa que verifique si un carácter es una letra mayúscula O una letra minúscula.
**Pista:** Usa `char >= 'A' && char <= 'Z'` para mayúsculas

## Ejercicios Intermedios (9-16)

### 9. Sistema de descuentos
Escribe un programa que aplique descuento si el cliente es VIP O compra más de $500.
**Pista:** Usa variables booleanas para VIP y monto de compra

### 10. Verificar triángulo válido
Crea un programa que determine si tres lados pueden formar un triángulo (cada lado debe ser menor que la suma de los otros dos).
**Pista:** Necesitas tres condiciones unidas por &&: `a < b + c && b < a + c && c < a + b`

### 11. Validar fecha simple
Escribe un programa que verifique si un día es válido para un mes (considera solo meses de 30 días).
**Pista:** `dia >= 1 && dia <= 30`

### 12. Sistema de acceso por horario
Crea un programa que permita acceso si es horario laboral (9-17 horas) Y no es fin de semana.
**Pista:** Combina verificación de hora con día de semana

### 13. Calculadora de IMC con categorías
Escribe un programa que determine si una persona tiene peso normal (IMC entre 18.5 y 24.9) O sobrepeso (IMC entre 25 y 29.9).
**Pista:** Calcula IMC primero, luego usa rangos con &&

### 14. Verificar contraseña segura
Crea un programa que verifique si una contraseña tiene al menos 8 caracteres Y contiene al menos un número.
**Pista:** Usa `contraseña.Length >= 8` y un bucle para buscar dígitos

### 15. Sistema de calificaciones
Escribe un programa que determine si un estudiante tiene beca (promedio >= 8.5 Y sin materias reprobadas).
**Pista:** Usa variables para promedio y número de materias reprobadas

### 16. Verificar número primo simple
Crea un programa que verifique si un número menor a 100 es primo (solo verifica divisibilidad por 2 Y 3).
**Pista:** `numero > 1 && numero % 2 != 0 && numero % 3 != 0` (considera casos especiales para 2 y 3)

## Ejercicios Avanzados (17-24)

### 17. Sistema de login con intentos
Escribe un programa que permita login si las credenciales son correctas O si es el último intento permitido.
**Pista:** Usa contador de intentos y combina con verificación de credenciales

### 18. Validar coordenadas en cuadrante
Crea un programa que determine si un punto (x,y) está en el primer cuadrante O en el tercer cuadrante.
**Pista:** Primer cuadrante: `x > 0 && y > 0`, tercer cuadrante: `x < 0 && y < 0`

### 19. Sistema de temperatura de emergencia
Escribe un programa que active alarma si la temperatura es muy alta mayor 35°C O muy baja, menor 5°C Y el sistema está activo.
**Pista:** Agrupa las condiciones de temperatura con paréntesis

### 20. Verificar jugada de poker simple
Crea un programa que determine si tienes una pareja (dos cartas iguales) en una mano de 3 cartas.
**Pista:** Compara `carta1 == carta2 || carta1 == carta3 || carta2 == carta3`

### 21. Sistema de préstamo bancario
Escribe un programa que apruebe un préstamo si el ingreso es alto (>$5000) O si tiene buen historial crediticio Y ingreso moderado (>$2000).
**Pista:** Usa paréntesis para agrupar: `ingreso > 5000 || (buenHistorial && ingreso > 2000)`

### 22. Validar movimiento en juego
Crea un programa que verifique si un movimiento en un tablero es válido (dentro de límites Y la casilla está vacía).
**Pista:** `x >= 0 && x < 8 && y >= 0 && y < 8 && casilla == 0`

### 23. Sistema de notificaciones
Escribe un programa que envíe notificación si es horario permitido (8-22 horas) O es una emergencia Y el usuario acepta notificaciones nocturnas.
**Pista:** Combina múltiples condiciones con paréntesis para agrupar correctamente

### 24. Verificar secuencia ordenada
Crea un programa que determine si tres números están en orden ascendente O descendente.
**Pista:** `(a <= b && b <= c) || (a >= b && b >= c)`

---

## Consejos Generales:
- Usa paréntesis para aclarar el orden de las operaciones
- Recuerda que && tiene mayor precedencia que ||
- && se evalúa como "cortocircuito": si la primera condición es falsa, no evalúa la segunda
- || también es "cortocircuito": si la primera condición es verdadera, no evalúa la segunda
- Prueba tus programas con diferentes casos: verdadero-verdadero, verdadero-falso, falso-verdadero, falso-falso