# 🧠 Clase 6: Gestión de Memoria — El Arte de Organizar el Espacio Digital

## "La memoria del computador es como la biblioteca de Alejandría: todo debe estar perfectamente organizado para encontrarlo cuando se necesite"

## 👋 ¡Hola parceros y parceras tech de Medellín!
En la clase anterior exploramos cómo el sistema operativo gestiona los procesos. Hoy vamos a profundizar en **cómo se administra la memoria**: desde los diferentes tipos hasta las técnicas avanzadas de segmentación y paginación. Aprenderemos a monitorear el uso de memoria con herramientas reales y resolveremos casos prácticos.

---

## 🎯 Objetivos de Aprendizaje
Al finalizar esta clase (4 horas), ustedes podrán:
- ✅ Distinguir los tipos de memoria y su jerarquía (RAM, ROM, caché, virtual)
- ✅ Explicar técnicas de gestión: segmentación, paginación y memoria virtual
- ✅ Calcular direccionamiento en segmentación y traducción de páginas
- ✅ Analizar políticas de reemplazo de páginas (FIFO, LRU, Optimal)
- ✅ Monitorear uso de memoria con herramientas del sistema
- ✅ Resolver casos prácticos de optimización de memoria
- ✅ Realizar ejercicios de organización y asignación de memoria

---

## 🧭 Cronograma de la Clase (4 horas)
| Bloque | Duración | Actividad | Propósito |
|--------|----------|-----------|-----------|
| 1 | 15 min | Activación + repaso gestión procesos | Conectar conocimientos |
| 2 | 35 min | Jerarquía y tipos de memoria | Marco conceptual |
| 3 | 40 min | Segmentación: conceptos y ejercicios | Técnica básica |
| 4 | 40 min | Paginación y memoria virtual | Técnica avanzada |
| 5 | 30 min | Políticas de reemplazo de páginas | Algoritmos de gestión |
| 6 | 35 min | Monitoreo con herramientas del sistema | Práctica real |
| 7 | 35 min | Taller: Ejercicios de organización | Aplicación práctica |
| 8 | 25 min | Resolución de casos de uso | Pensamiento crítico |
| 9 | 5 min | Evaluación + cierre | Consolidación |

---

## 🔄 Activación: Repaso y Conexión (15 min)

### Quiz Rápido de Conexión
1. ¿Qué información guarda el PCB sobre la memoria de un proceso?
2. ¿Por qué un proceso puede estar en estado "Blocked/Waiting"?
3. ¿Qué pasa cuando un proceso necesita más memoria de la disponible?

### Analogía de Apertura
La gestión de memoria es como **organizar los libros en una biblioteca**:
- **RAM:** Los libros en los estantes de consulta rápida
- **Almacenamiento:** El almacén con todos los libros
- **Caché:** Los libros más consultados en el escritorio del bibliotecario
- **Memoria Virtual:** Un sistema que simula tener más estantes de los físicos

---

## 🏗️ Jerarquía y Tipos de Memoria (35 min)

### 📊 Pirámide de la Jerarquía de Memoria
```
    [Registros CPU] ← Más rápida, más cara
         [Caché L1/L2/L3]
              [RAM (Memoria Principal)]
                   [SSD/Disco Duro]
                        [Almacenamiento en Nube] ← Más lenta, más barata
```

### Tipos de Memoria Principales

#### **1. ROM (Read-Only Memory)**
- **Función:** Almacena firmware del sistema (BIOS/UEFI)
- **Características:** No volátil, solo lectura, pequeña capacidad
- **Ejemplo local:** Como la cédula de ciudadanía - información que no cambia

#### **2. RAM (Random Access Memory)**
- **Función:** Memoria principal de trabajo para procesos activos
- **Tipos principales:**
  - **DRAM:** Más barata, necesita refresh constante
  - **SRAM:** Más rápida, usada en caché, más costosa
- **Características:** Volátil, acceso aleatorio rápido
- **Analogía:** Como el escritorio donde trabajas - lo que necesitas ahora

#### **3. Memoria Caché**
- **Niveles:** L1 (más rápida/pequeña) → L2 → L3 (más lenta/grande)
- **Principio:** Localidad temporal y espacial
- **Hit/Miss:** ¿Los datos están en caché o hay que buscarlos en RAM?
- **Ejemplo:** Como tener los números telefónicos más usados en marcación rápida

#### **4. Memoria Virtual**
- **Concepto:** Simular más memoria RAM usando almacenamiento secundario
- **Ventajas:** Ejecutar programas más grandes que la RAM física
- **Swap/Paging:** Intercambio de páginas entre RAM y disco

### 🔧 Métricas de Rendimiento
| Tipo | Velocidad | Capacidad | Costo/GB | Volatilidad |
|------|-----------|-----------|----------|-------------|
| Registros | ~1 ns | Bytes | N/A | Volátil |
| Caché L1 | ~2-4 ns | KB | Muy alto | Volátil |
| RAM | ~100 ns | GB | Medio | Volátil |
| SSD | ~100 μs | TB | Bajo | No volátil |
| HDD | ~10 ms | TB | Muy bajo | No volátil |

---

## 🧩 Segmentación: Dividir por Funciones (40 min)

### Concepto de Segmentación
La **segmentación** divide la memoria del proceso en segmentos lógicos según su función:
- **Segmento de Código:** Instrucciones del programa
- **Segmento de Datos:** Variables globales e inicializadas
- **Segmento de Pila (Stack):** Variables locales y llamadas a funciones
- **Segmento de Heap:** Memoria dinámica (malloc, new)

### Tabla de Segmentos
| Segmento | Base | Límite | Permisos |
|----------|------|--------|----------|
| Código | 1000 | 2000 | R-X |
| Datos | 3000 | 1500 | RW- |
| Pila | 8000 | 2000 | RW- |
| Heap | 5000 | 3000 | RW- |

### Cálculo de Dirección Física
**Fórmula:** Dirección Física = Base + Desplazamiento

**Ejemplo práctico:**
- Dirección lógica: Segmento 1, Desplazamiento 500
- Tabla: Segmento 1 (Datos) → Base = 3000, Límite = 1500
- ¿Válida? 500 < 1500 ✅
- Dirección física: 3000 + 500 = 3500

### 🎮 Ejercicio Grupal (15 min)
En parejas, resolver:
1. Proceso con 4 segmentos, calcular 5 direcciones físicas
2. Identificar violaciones de límites
3. Discutir ventajas de segmentación (protección, compartición)

### Ventajas y Desventajas
**✅ Ventajas:**
- Protección natural entre segmentos
- Fácil compartición de código
- Crecimiento dinámico de segmentos

**❌ Desventajas:**
- Fragmentación externa
- Gestión compleja de tamaños variables

---

## 📄 Paginación y Memoria Virtual (40 min)

### Concepto de Paginación
La **paginación** divide la memoria en bloques de tamaño fijo llamados **páginas** (memoria lógica) y **marcos** (memoria física).

### Características Clave
- **Tamaño de página:** Típicamente 4KB, 8KB o 16KB
- **Sin fragmentación externa:** Todos los bloques son del mismo tamaño
- **Fragmentación interna:** Solo el último bloque puede no llenarse completamente

### Tabla de Páginas
| Página Lógica | Marco Físico | Bit Válido | Permisos |
|---------------|--------------|-------------|----------|
| 0 | 3 | 1 | RW |
| 1 | 7 | 1 | R- |
| 2 | 1 | 1 | RWX |
| 3 | - | 0 | - |

### Traducción de Direcciones
**Dirección lógica** = Número de página + Desplazamiento
**Dirección física** = Marco físico + Desplazamiento

**Ejemplo con páginas de 1KB (1024 bytes):**
- Dirección lógica: 3500
- Página: 3500 ÷ 1024 = 3 (página lógica)
- Desplazamiento: 3500 % 1024 = 412
- Marco físico: Tabla[3] = No válido → **Page Fault!**

### 🔄 Page Fault y Memoria Virtual
Cuando una página no está en RAM:
1. **Interrupción de page fault**
2. **SO busca la página en almacenamiento secundario**
3. **Carga la página en un marco libre**
4. **Actualiza la tabla de páginas**
5. **Reinicia la instrucción**

### TLB (Translation Lookaside Buffer)
- **Caché de traducciones** más frecuentes
- **Hit TLB:** Traducción directa y rápida
- **Miss TLB:** Buscar en tabla de páginas

---

## 🔄 Políticas de Reemplazo de Páginas (30 min)

### El Problema
Cuando la RAM está llena y se necesita cargar una nueva página, **¿cuál página remover?**

### Algoritmos de Reemplazo

#### **1. FIFO (First In, First Out)**
- **Estrategia:** Remover la página que llegó primero
- **Ventaja:** Simple de implementar
- **Desventaja:** No considera frecuencia de uso
- **Anomalía de Belady:** Más marcos pueden generar más page faults

#### **2. LRU (Least Recently Used)**
- **Estrategia:** Remover la página usada menos recientemente
- **Ventaja:** Considera localidad temporal
- **Implementación:** Stack o bits de referencia

#### **3. Optimal (OPT)**
- **Estrategia:** Remover la página que se usará más tarde en el futuro
- **Problema:** Requiere conocimiento del futuro (solo para comparación teórica)

### 📊 Ejercicio Comparativo (15 min)
**Secuencia de referencias:** 7, 0, 1, 2, 0, 3, 0, 4, 2, 3, 0, 3, 2, 1, 2, 0, 1, 7, 0, 1
**Marcos disponibles:** 3

| Algoritmo | Page Faults | Hit Rate |
|-----------|-------------|----------|
| FIFO | | |
| LRU | | |
| Optimal | | |

Los estudiantes completan en grupos y comparan resultados.

---

## 🖥️ Monitoreo con Herramientas del Sistema (35 min)

### Herramientas en Windows

#### **Administrador de Tareas**
1. **Pestaña Rendimiento → Memoria:**
   - Memoria en uso vs disponible
   - Memoria comprometida
   - Pool paginado/no paginado

2. **Pestaña Procesos:**
   - Memoria privada por proceso
   - Conjunto de trabajo (Working Set)

#### **Monitor de Recursos (resmon.exe)**
- **Vista detallada de uso por proceso**
- **Errores de página por segundo**
- **E/S de memoria virtual**

### Herramientas en Linux

#### **Comando `free`**
```bash
$ free -h
              total        used        free      shared  buff/cache   available
Mem:           7.7G        2.1G        1.2G        284M        4.4G        5.1G
Swap:          2.0G          0B        2.0G
```

#### **Comando `top` / `htop`**
- **Métricas:** %MEM, RES (memoria residente), VIRT (memoria virtual)
- **Swap usage:** Cuánto se está usando memoria virtual

#### **Archivo `/proc/meminfo`**
```bash
$ cat /proc/meminfo | head -10
MemTotal:        7943920 kB
MemFree:         1245680 kB
MemAvailable:    5234560 kB
Buffers:          156840 kB
Cached:          4193280 kB
```

### 🔍 Actividad Práctica Guiada (20 min)
1. **Abrir varias aplicaciones** (navegador, editor, calculadora)
2. **Monitorear el cambio en uso de memoria**
3. **Identificar procesos que más consumen**
4. **Observar swap/paging** cuando se agota RAM
5. **Documentar hallazgos** en plantilla

**Plantilla de observación:**
| Aplicación | RAM Inicial | RAM Final | Swap Usado | Page Faults |
|------------|-------------|-----------|------------|-------------|
| Sistema base | | | | |
| Navegador | | | | |
| + Editor texto | | | | |
| + Calculadora | | | | |

---

## 🧪 Taller: Ejercicios de Organización de Memoria (35 min)

### Ejercicio 1: Segmentación Manual (15 min)
**Escenario:** Proceso con 4 segmentos en sistema con 16KB de RAM

**Tabla de segmentos:**
| Segmento | Tamaño | Base | Límite |
|----------|--------|------|--------|
| Código | 3KB | 0 | 3071 |
| Datos | 2KB | 4096 | 2047 |
| Pila | 1KB | 8192 | 1023 |
| Heap | 2KB | 12288 | 2047 |

**Calcular direcciones físicas:**
1. Código, offset 1500
2. Datos, offset 500
3. Pila, offset 2000 (¿error?)
4. Heap, offset 1000

### Ejercicio 2: Paginación Práctica (20 min)
**Sistema:** Páginas de 1KB, 4 marcos de memoria física

**Escenario:** Proceso de 5KB necesita ejecutarse
- **Página 0:** Marco 2
- **Página 1:** Marco 0  
- **Página 2:** No cargada
- **Página 3:** Marco 3
- **Página 4:** Marco 1

**Referencias de memoria:** 0, 1200, 2500, 3800, 4100, 800

Para cada referencia:
1. ¿Qué página lógica?
2. ¿Está en memoria?
3. Si sí, ¿dirección física?
4. Si no, ¿page fault?

### Soluciones y Discusión
Revisión grupal con explicación en pizarra de cada caso.

---

## 🎯 Resolución de Casos de Uso (25 min)

### Caso 1: "PC Lento en el Colegio"
**Situación:** Computador del laboratorio con 4GB RAM ejecuta muy lento cuando los estudiantes abren múltiples aplicaciones.

**Síntomas observados:**
- LED de disco duro siempre activo
- Respuesta lenta al cambiar entre aplicaciones
- Sonido constante de acceso a disco

**Preguntas guía:**
1. ¿Qué está pasando con la memoria?
2. ¿Cómo lo confirmarías con herramientas?
3. ¿Qué soluciones inmediatas propones?
4. ¿Qué soluciones a largo plazo?

### Caso 2: "App Móvil que se Cierra Sola"
**Situación:** App de juego en Android se cierra cuando recibes un WhatsApp.

**Análisis:**
1. ¿Por qué Android mata procesos?
2. ¿Qué criterios usa?
3. ¿Cómo priorizaría los procesos?

### Caso 3: "Servidor Web Sobrecargado"
**Situación:** Servidor web de un colegio se vuelve muy lento durante exámenes en línea.

**Datos:**
- 100 estudiantes simultáneos
- Servidor: 8GB RAM
- Cada sesión: ~50MB promedio

**Análisis requerido:**
1. Cálculo de memoria necesaria
2. Identificación del cuello de botella
3. Estrategias de optimización

---

## 📝 Evaluación Rápida (5 min)

### Quiz Final
1. **¿Cuál es la diferencia entre segmentación y paginación?**
2. **¿Qué causa un page fault?**
3. **¿Por qué LRU es mejor que FIFO para reemplazo de páginas?**
4. **¿Cómo identificas que un sistema está usando mucho swap?**
5. **¿Qué comando de Linux muestra el uso detallado de memoria?**

---

## 📚 Recursos Adicionales

### Herramientas de Simulación
- **Simulador de paginación online:** OS Virtual Memory Simulator
- **Calculadora de direcciones:** Memory Management Calculator
- **Visualizador de algoritmos:** Algorithm Visualizer (LRU, FIFO)

### Comandos Útiles
**Linux:**
```bash
# Información de memoria
free -h
cat /proc/meminfo
vmstat 1

# Procesos y memoria
top
htop
ps aux --sort=-%mem

# Información de swap
swapon -s
cat /proc/swaps
```

**Windows:**
```cmd
# Información de memoria
wmic computersystem get TotalPhysicalMemory
wmic OS get TotalVisibleMemorySize

# Monitor de rendimiento
perfmon
resmon
```

### Lecturas Recomendadas
- Tanenbaum - Capítulo 3: Memory Management
- Silberschatz - Capítulo 8: Main Memory y Capítulo 9: Virtual Memory
- Documentación del kernel Linux sobre memoria virtual

---

## 🏆 Evaluación de la Clase

### Distribución de Calificación
| Componente | Peso | Criterios |
|------------|------|-----------|
| Ejercicios de segmentación | 25% | Cálculos correctos + comprensión |
| Ejercicios de paginación | 25% | Traducción de direcciones + page faults |
| Actividad de monitoreo | 20% | Uso correcto de herramientas + observaciones |
| Casos de uso | 20% | Análisis y propuestas de solución |
| Quiz final | 10% | Conceptos clave |

### Criterios de Excelencia
- **Sobresaliente (4.5-5.0):** Domina conceptos, resuelve problemas complejos, propone optimizaciones
- **Notable (4.0-4.4):** Buen manejo de conceptos, resuelve ejercicios con apoyo mínimo
- **Satisfactorio (3.5-3.9):** Comprende conceptos básicos, necesita guía en ejercicios
- **Mejorable (3.0-3.4):** Conceptos confusos, dificultades en aplicación práctica

---

## 🌟 Proyecto de Extensión

### "Auditoría de Memoria en Mi Equipo"
**Objetivo:** Analizar el uso de memoria de un computador personal durante una semana.

**Entregables:**
1. **Reporte de baseline:** Estado inicial del sistema
2. **Log de monitoreo:** Uso de memoria en diferentes momentos del día
3. **Análisis de aplicaciones:** Qué consume más memoria y por qué
4. **Propuestas de optimización:** Cómo mejorar el rendimiento

**Herramientas sugeridas:**
- Administrador de Tareas (Windows) / htop (Linux)
- HWiNFO64, CPU-Z para información detallada de hardware
- Aplicaciones de monitoreo continuo (opcional)

**Formato:** Informe de 2-3 páginas con capturas de pantalla y gráficos

---

## 💡 Tips Finales para Estudiantes

1. **Observa patrones:** La memoria se comporta de forma predecible
2. **Usa las herramientas:** El sistema te dice exactamente qué está pasando
3. **Piensa en trade-offs:** Más memoria = más velocidad, pero más costo
4. **Contextualiza localmente:** ¿Cómo optimizarías un computador para una biblioteca pública de Medellín?

---

## 🎬 Reflexión Final

La gestión de memoria es como **administrar los recursos de una ciudad**: hay que optimizar el uso del espacio limitado, predecir necesidades futuras, y mantener todo funcionando sin desperdiciar recursos.

**Frase de cierre:** *"La memoria perfectamente gestionada es invisible para el usuario, pero fundamental para la experiencia"*

¡Nos vemos en la próxima clase donde exploraremos la gestión de archivos y sistemas de almacenamiento! 📁🔧

---

**¡Hasta la próxima, gestores de memoria de Medellín!** 🧠⚡
