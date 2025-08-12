# 🖥️📱 Clase 3: Tipos de Sistemas Operativos (4 horas)

## "El universo de los Sistemas Operativos: ¿Dónde viven y para qué sirven?"

## 👋 ¡Hola parceros y parceras tech de Medellín!
En las clases anteriores entendimos qué es un sistema operativo, sus componentes y funciones internas. Hoy vamos a explorar los **tipos de sistemas operativos** que existen en distintos dispositivos y contextos: desde tu computador personal hasta los controladores que operan semáforos, robots, drones o el Metro de Medellín.

Vamos a descubrir cómo cada tipo está diseñado con **propósitos específicos**, qué los hace únicos y en qué escenarios se usan. Además, trabajaremos en una **mesa redonda** y diseñaremos **infografías temáticas** para reforzar lo aprendido.

---

## 🎯 Objetivos de Aprendizaje
Al finalizar esta clase (4 horas), ustedes podrán:
- ✅ Diferenciar los principales tipos de sistemas operativos: **de escritorio, móviles, embebidos, en red y de tiempo real (RTOS)**
- ✅ Identificar características clave y componentes más relevantes de cada tipo
- ✅ Relacionar ejemplos reales y su contexto de uso (local y global)
- ✅ Analizar ventajas y limitaciones según el ámbito de aplicación
- ✅ Participar en una mesa redonda argumentando con criterios técnicos
- ✅ Diseñar una infografía clara, atractiva y rigurosa sobre un tipo de SO

---

## 🧭 Ruta General de la Clase (240 min)
| Bloque | Duración | Actividad | Propósito |
|--------|----------|-----------|-----------|
| 1 | 25 min | Activación y repaso | Conectar saberes previos |
| 2 | 40 min | Introducción conceptual a los tipos | Marco teórico base |
| 3 | 35 min | Análisis comparativo guiado | Profundización crítica |
| 4 | 30 min | Estudio de casos reales | Aplicación contextual |
| 5 | 35 min | Mesa redonda (debate técnico) | Argumentación y pensamiento crítico |
| 6 | 55 min | Taller: Diseño de infografías | Síntesis creativa |
| 7 | 20 min | Socialización y feedback | Aprendizaje entre pares |
| 8 | 10 min | Cierre y reflexión | Metacognición |
| Extra | (Integrado) | Evaluación formativa continua | Observación + rúbricas |

---

## 🧪 Activación y Repaso (Cuestionario Diagnóstico) {#activacion}
**Duración sugerida:** 20–25 min  
**Propósito:** Activar conocimientos clave de la Clase 2 (componentes y funciones del SO) para construir sobre bases sólidas.

### Estructura
| Sección | Tipo | Ítems | Tiempo |
|---------|------|-------|--------|
| 1 | Selección múltiple | 8 | 6 min |
| 2 | Verdadero/Falso | 6 | 4 min |
| 3 | Relacionar | 5 | 4 min |
| 4 | Respuesta corta | 5 | 6 min |
| 5 | Caso práctico | 1 | 3–4 min |
| 6 | Autoevaluación | 3 | 2 min |

### Sección 1: Selección Múltiple
1. El componente que decide qué proceso usa el CPU: a) Gestor usuarios b) Sistema de archivos c) Planificador de procesos d) Controlador hardware  
2. Mover datos de RAM a disco para liberar espacio: a) Caché gráfico b) Swapping c) Clustering d) Refresco  
3. ¿Qué NO es de almacenamiento? a) Organización carpetas b) Permisos archivos c) Planificación CPU d) Respaldo  
4. Un sistema multiusuario permite: a) Un proceso b) Varios usuarios simultáneos c) Menos seguridad d) Sin memoria virtual  
5. Ventaja típica de Linux en servidores: a) Más licencias b) Código abierto y estabilidad c) Menos redes d) No multiusuario  
6. Memoria virtual es: a) Nube multimedia b) Simular más RAM con disco c) Duplicar procesos d) Solo móvil  
7. Multitarea preventiva: a) Ceden voluntario b) Planificador interrumpe c) Solo embebidos d) Sin múltiples apps  
8. Android destaca por: a) Servidores bancarios b) Ecosistema móvil + gestión recursos c) Sin permisos d) No multitarea  

### Sección 2: Verdadero / Falso
1. ( ) El kernel coordina hardware y procesos  
2. ( ) Monoproceso = varias apps simultáneas  
3. ( ) Protección de memoria separa procesos  
4. ( ) NTFS y ext4 son gestores de procesos  
5. ( ) Multiusuario: sesiones independientes  
6. ( ) Auditoría registra acciones usuarios  

### Sección 3: Relacionar
1. Swapping  
2. Sistema de archivos  
3. Autenticación  
4. IPC  
5. Memoria virtual  

Descripciones:
A. Control de acceso a archivos  
B. Mover procesos entre RAM y disco  
C. Verificar identidad usuario  
D. Comunicación entre procesos  
E. Simular más memoria disponible  

### Sección 4: Respuesta Corta
1. Diferencia monoproceso vs multiproceso.  
2. Una función crítica de gestión de usuarios.  
3. Por qué es útil la memoria virtual.  
4. Ejemplo de multitarea en tu teléfono.  
5. Ventaja de multiusuario en laboratorio escolar.  

### Sección 5: Caso Práctico
Escenario: Música + descarga grande + edición documento + videollamada. Equipo se ralentiza.
1. ¿Quién decide turnos CPU?  
2. ¿Qué libera RAM moviendo a disco?  
3. Al cerrar la app menos prioritaria, ¿qué gestión aplicas?  
4. ¿Riesgo sin protección de memoria?  

### Sección 6: Autoevaluación (1–5)
| Tema | 1 | 2 | 3 | 4 | 5 |
|------|---|---|---|---|---|
| Kernel | | | | | |
| Procesos | | | | | |
| Memoria | | | | | |
| Archivos | | | | | |
| Mono vs Multi | | | | | |
| Windows/Linux/Android | | | | | |

### (Opcional) Bonus
¿Por qué un SO móvil cierra o suspende más agresivamente apps en segundo plano que uno de escritorio?

> Nota docente (ocultar a estudiantes): Clave resumida: 1c 2b 3c 4b 5b 6b 7b 8b / V F V F V V / Rel: 1B 2A 3C 4D 5E.

---

## 🏷️ Tipos de Sistemas Operativos a Estudiar
1. **Sistemas Operativos de Escritorio (Desktop)**
2. **Sistemas Operativos Móviles**
3. **Sistemas Operativos Embebidos (Embedded)**
4. **Sistemas Operativos en Red / Distribuidos**
5. **Sistemas Operativos de Tiempo Real (RTOS)**

---

## 1. 💻 Sistemas Operativos de Escritorio
Pensados para computadoras personales de uso general: productividad, navegación, multimedia, desarrollo.

### Ejemplos:
- Windows 10/11
- Ubuntu (Linux) / Linux Mint / Fedora
- macOS (Apple)

### Características Clave:
- Interfaz gráfica rica (ventanas, escritorios virtuales)
- Multitarea y multiusuario
- Soporte amplio de periféricos y drivers
- Gestión avanzada de archivos y seguridad (permisos, usuarios)

### Ámbitos de Aplicación:
- Hogares, oficinas, diseño gráfico, programación, educación.

### Analogía local:
Como el **Parque Explora**: un lugar versátil donde se pueden hacer muchas actividades diferentes.

---

## 2. 📱 Sistemas Operativos Móviles
Optimizados para dispositivos portátiles con recursos energéticos limitados y orientados a interacción táctil.

### Ejemplos:
- Android
- iOS
- HarmonyOS

### Características Clave:
- Interfaz touch-first (gestos, notificaciones push)
- Gestión agresiva de energía y procesos en segundo plano
- Enfoque en conectividad (4G/5G, WiFi, GPS, sensores)
- Ecosistemas de apps y permisos granulares

### Ámbitos de Aplicación:
- Smartphones, tablets, relojes inteligentes.

### Analogía local:
Como el **MetroCable**: eficiente, optimizado y diseñado para movilidad constante.

---

## 3. ⚙️ Sistemas Operativos Embebidos
Incluidos dentro de dispositivos específicos para realizar una o pocas funciones críticas de forma eficiente y confiable.

### Ejemplos:
- Firmware de un router (OpenWrt)
- Controladores de cajeros automáticos (ATM)
- Microcontroladores con FreeRTOS / Zephyr
- Sistemas de paneles solares o termostatos
- ECU en motos eléctricas o carros

### Características Clave:
- Consumo mínimo de recursos (memoria, CPU, energía)
- Funcionalidad específica (no uso general)
- Alta estabilidad y baja interacción directa con usuario
- A veces sin interfaz gráfica (solo LEDs / pantallas simples)

### Ámbitos de Aplicación:
- Domótica, electrodomésticos, IoT, automoción, salud.

### Analogía local:
Como una **máquina de boletería del Metro**: hace una tarea precisa, fiable y repetible.

---

## 4. 🌐 Sistemas Operativos en Red / Distribuidos
Diseñados para gestionar recursos compartidos entre múltiples computadoras conectadas.

### Ejemplos:
- Linux en servidores (Ubuntu Server, CentOS, Debian)
- Windows Server
- Sistemas distribuidos como Kubernetes (orquestación sobre un conjunto de nodos Linux)
- Network OS en switches/routers (Cisco IOS, JunOS)

### Características Clave:
- Compartición de recursos (archivos, usuarios, impresoras, servicios)
- Escalabilidad y administración centralizada
- Servicios de autenticación (LDAP, Active Directory)
- Alta disponibilidad y redundancia

### Ámbitos de Aplicación:
- Servidores web, bases de datos, servicios en la nube, infraestructura de ciudad inteligente.

### Analogía local:
Como la **central de control del Metro de Medellín**: coordina múltiples líneas y estaciones para un servicio integrado.

---

## 5. ⏱️ Sistemas Operativos de Tiempo Real (RTOS)
Garantizan respuestas dentro de un tiempo máximo predecible. Usados en sistemas críticos donde un retraso puede causar fallos graves.

### Ejemplos:
- FreeRTOS
- VxWorks
- QNX
- RTLinux (variantes con parches en tiempo real)
- Sistemas de drones, robots industriales, dispositivos médicos

### Características Clave:
- Determinismo (tiempos de respuesta predecibles)
- Planificación prioritaria estricta
- Uso eficiente de interrupciones
- Seguridad y confiabilidad elevadas

### Ámbitos de Aplicación:
- Automatización industrial, aeronáutica, automoción, salud, telecomunicaciones.

### Analogía local:
Como los **semáforos inteligentes sincronizados**: deben responder en tiempos exactos para evitar caos.

---

## 🧪 Tabla Comparativa de Tipos
| Tipo | Interfaz | Recursos | Flexibilidad | Tiempo Crítico | Ejemplos | Riesgo si falla |
|------|----------|----------|-------------|---------------|----------|-----------------|
| Escritorio | Compleja / GUI | Altos | Alta | Medio | Windows, Ubuntu, macOS | Pérdida productividad |
| Móvil | Touch / GUI | Medios-Limitados | Media | Medio | Android, iOS | Pérdida comunicación |
| Embebido | Mínima / None | Muy bajos | Baja | Variable | Firmware router, IoT | Fallo del dispositivo |
| En Red | CLI/GUI | Escalables | Alta | Medio | Linux Server, Windows Server | Corte de servicios |
| Tiempo Real | Muy específica | Ajustados | Baja-Media | Alto (determinista) | FreeRTOS, QNX | Riesgo operativo / seguridad |

---

## 🔍 Estudio de Casos (Mini Fichas)
### Caso 1: Android en Smartphones
- Problema que resuelve: Integrar comunicación, multimedia y apps en un dispositivo portátil.
- Reto técnico: Batería limitada y diversidad de hardware.
- Clave: Gestión dinámica de procesos (kill / suspend) y permisos.

### Caso 2: FreeRTOS en Drones
- Problema: Controlar motores y sensores en microsegundos.
- Reto: Latencia mínima y sincronización.
- Clave: Tareas con prioridades rígidas y timers precisos.

### Caso 3: Linux Server en un Portal Web Escolar
- Problema: Atender múltiples solicitudes de estudiantes y docentes.
- Reto: Escalabilidad y seguridad.
- Clave: Gestión de procesos y servicios (Nginx, Apache, DB, SSH).

### Caso 4: Firmware de Semáforo Inteligente
- Problema: Regular flujo vehicular adaptado a horarios.
- Reto: Ciclos temporizados confiables.
- Clave: RTOS o loop embebido con interrupciones.

### Caso 5: macOS para Diseño Gráfico
- Problema: Flujo de trabajo creativo de alta calidad.
- Reto: Estabilidad y rendimiento en multimedia.
- Clave: Integración hardware-software optimizada.

---

## 🧠 Pensamiento Crítico (Preguntas Guía)
1. ¿Por qué no se instala Android en un servidor web?
2. ¿Qué pasaría si un RTOS se comportara como un SO de escritorio en una máquina médica?
3. ¿Qué ventajas trae que los SO embebidos sean minimalistas?
4. ¿Cómo afecta la conectividad a los sistemas operativos en red?
5. ¿En qué casos un SO móvil se parece a uno de escritorio hoy en día?

---

## 🗣️ Actividad Central 1: Mesa Redonda (Debate Técnico)
**Duración:** 35 minutos

### Objetivo:
Desarrollar habilidades de argumentación comparando tipos de sistemas operativos según un escenario planteado.

### Escenario del Debate:
"La Alcaldía de Medellín planea un sistema inteligente para movilidad, educación y salud conectada. ¿Qué combinación de tipos de SO es más adecuada y por qué?"

### Roles Sugeridos (asignar grupos):
- Equipo Escritorio
- Equipo Móvil
- Equipo Embebido
- Equipo Red / Distribuido
- Equipo Tiempo Real

### Fases:
1. Preparación (10 min): Cada equipo formula 3 argumentos a favor y 1 limitación propia.
2. Exposición (10 min): 2 min por equipo.
3. Ronda de Preguntas Cruzadas (10 min): Cada equipo pregunta a otro.
4. Cierre y Síntesis (5 min): El docente o moderador recoge conclusiones.

### Criterios de Evaluación (Rúbrica rápida):
- Claridad técnica (0-3)
- Relevancia de ejemplos (0-3)
- Trabajo colaborativo (0-2)
- Capacidad de responder preguntas (0-2)

---

## 🎨 Actividad Central 2: Taller de Infografías Temáticas
**Duración Total:** 55 minutos

### Objetivo:
Sintetizar y comunicar visualmente la información clave sobre un tipo de sistema operativo.

### Entregable:
Una infografía (digital o en cartulina) que responda: ¿Qué es? ¿Cómo funciona? ¿Dónde se usa? ¿Por qué importa?

### Estructura Recomendada:
1. Título atractivo (ej: "RTOS: El Tiempo es Vida")
2. Definición breve (máx. 30 palabras)
3. 3-5 características visuales (iconos/colores)
4. Ejemplos reales (logos o pictogramas)
5. Caso local (ejemplo Medellín / Colombia)
6. Ventajas y limitaciones (balance visual)
7. Futuro / tendencia (1 frase)
8. Fuente / Referencias

### Herramientas Sugeridas:
- Digital: Canva, Google Slides, Genially
- Analógico: Cartulinas, marcadores, post-its

### Proceso (pasos y tiempo):
- Investigación breve guiada: 10 min
- Boceto (wireframe): 10 min
- Construcción: 25 min
- Ajustes finales: 10 min

### Criterios de Evaluación (Rúbrica):
| Criterio | Excelente (3) | Bueno (2) | Básico (1) |
|----------|---------------|----------|-----------|
| Claridad conceptual | Preciso y completo | Mayormente claro | Incompleto |
| Diseño visual | Muy atractivo y organizado | Adecuado | Confuso |
| Uso de ejemplos | Relevantes y variados | Correctos pero pocos | Escasos |
| Creatividad | Innovador | Interesante | Limitada |
| Referencias | Citadas correctamente | Algunas | Ausentes |

Puntaje máximo: 15.

---

## ✍️ Actividad Complementaria: Clasificación Relámpago
**Duración:** 10 min (entre bloques)

El docente muestra (o describe) dispositivos y los estudiantes clasifican rápidamente el tipo de SO implicado:
- Cajero automático
- Smartwatch
- Cámara de seguridad IP
- Servidor web escolar
- Consola de videojuegos portátil
- Sensor de riego automático
- Tablet de dibujo

Reflexión: ¿Algún dispositivo usa más de un tipo de sistema operativo en su ecosistema?

---

## 📊 Matriz de Selección (Ejercicio Rápido)
Completar en parejas:
| Caso | Tipo Recomendado | Justificación corta |
|------|------------------|----------------------|
| Control de un brazo robótico | | |
| Plataforma educativa en línea | | |
| App de movilidad urbana integrada | | |
| Dron para entrega de paquetes | | |
| Panel de monitoreo de energía solar | | |
| Sistema de tickets Metro de Medellín | | |
| Monitor de signos vitales hospitalario | | |

---

## 🧩 Mini Quiz Diagnóstico (Opcional - 8 min)
1. ¿Qué tipo de SO prioriza tiempos de respuesta estrictos?  
2. ¿Cuál está más orientado a consumo mínimo de energía y memoria?  
3. Ejemplo de SO de red usado en empresas.  
4. ¿Qué diferencia principal hay entre un SO móvil y uno de escritorio?  
5. ¿Por qué un RTOS no usa una interfaz gráfica compleja normalmente?  

Respuestas sugeridas: 1. Tiempo real 2. Embebido 3. Windows Server / Linux Server 4. Optimización para energía y movilidad + interfaz táctil 5. Evita latencia y consumo de recursos.

---

## 🧱 Posibles Dificultades y Estrategias
| Dificultad | Estrategia de Apoyo |
|------------|--------------------|
| Confusión entre embebido y tiempo real | Mostrar que un embebido puede o no ser RTOS |
| Mezcla de ejemplos de servidor con escritorio | Diferenciar por función y escalabilidad |
| Exceso de texto en infografías | Limitar caracteres y usar iconos |
| Falta de argumentación en mesa redonda | Plantillas de argumento (Afirmación + Evidencia + Ejemplo) |

---

## 📚 Recursos Sugeridos
- Sitios oficiales: ubuntu.com, android.com, freertos.org
- Videos: Crash Course Computer Science (episodio OS), Platzi (introducción a IoT), canales de Raspberry Pi
- Herramientas: VirtualBox (probar distros), Emuladores Android, Simuladores FreeRTOS
- Local: Ruta N, Laboratorios UdeA, Makers Medellín, ferias STEAM escolares

---

## 🔭 Proyecto Extensión (Para Casa)
"Mapa Ecosistema Urbano Inteligente": Diseñar un esquema de sistemas operativos que podrían integrarse para una ciudad inteligente sostenible en Medellín (movilidad, salud, energía, educación).

Entregable: Diagrama + explicación (máx. 1 página o diapositiva). Incluir al menos 5 tipos de dispositivos y justificar qué tipo de SO usar en cada uno.

---

## 🧘 Cierre y Reflexión (Últimos 10 min)
Preguntas para el grupo:
1. ¿Qué tipo de SO te gustaría aprender a instalar o programar y por qué?
2. ¿Qué impacto social tiene elegir buenos sistemas operativos en servicios públicos?
3. ¿Cómo cambia tu visión al saber que hay SO invisibles trabajando todo el tiempo?

Frase de cierre: "No todos los sistemas operativos se ven, pero todos dejan huella en cómo vivimos la tecnología".

---

## 🏆 Evaluación
### Formativa (durante la sesión):
- Observación en mesa redonda (rúbrica)
- Progreso en boceto de infografía
- Participación en clasificación relámpago

### Sumativa (al final):
- Infografía (rúbrica 15 pts)
- Argumentos en mesa redonda (10 pts)
- Matriz de selección (5 pts)

Escala sugerida: 30 pts total.

---

## 💡 Tips para el Éxito
- Usa analogías locales para explicar conceptos técnicos.
- Resume antes de diseñar (no llenes la infografía de texto).
- Pregunta: ¿Qué problema específico resuelve este tipo de SO?
- Usa colores consistentes para categorías.
- En debate: respeta turnos, escucha, refuta con datos.

---

## 🌟 Bonus para Estudiantes Curiosos
- Investiga: ¿Qué es un hypervisor y cómo se relaciona con los SO?
- Explora Raspberry Pi VS Microcontrolador (Linux vs firmware ligero).
- Simula un dron en un entorno educativo y analiza su RTOS.

---

## 🙌 Despedida
Seguimos construyendo una visión amplia del mundo digital. Entender dónde vive cada tipo de sistema operativo nos prepara para **crear soluciones reales** para nuestra ciudad y el país.

Próxima clase: Profundizaremos en **seguridad y protección en sistemas operativos**. 🔒

---

¡Hasta la próxima, parceros! 🚀
