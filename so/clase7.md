# 📂 Clase 7: El Mapa del Mundo Digital — Sistemas de Archivos y la Consola

## "Para dominar el universo digital, primero debes aprender a navegarlo. La consola es tu brújula y el sistema de archivos es tu mapa."

## 👋 ¡Saludos, futuros arquitectos y arquitectas de la información!
En clases pasadas, desentrañamos los misterios de la memoria y los procesos. Hoy, vamos a poner los pies en la tierra, ¡literalmente en el disco duro! Exploraremos cómo los sistemas operativos organizan la información en **sistemas de archivos** y aprenderemos a movernos como expertos usando la **consola de comandos**, la herramienta más poderosa de un desarrollador.

---

## 🎯 Objetivos de Aprendizaje
Al finalizar esta clase (4 horas), ustedes podrán:
- ✅ Describir la estructura jerárquica de un sistema de archivos.
- ✅ Diferenciar las estructuras de archivos de Windows (letras de unidad) y Linux (raíz única).
- ✅ Navegar y manipular archivos y carpetas usando comandos esenciales en la consola.
- ✅ Comparar los comandos equivalentes entre Windows (CMD/PowerShell) y Linux (Bash).
- ✅ Crear y organizar estructuras de directorios para proyectos simulados.
- ✅ Resolver problemas prácticos utilizando la línea de comandos.

---

## 🧭 Cronograma de la Clase (4 horas)
| Bloque | Duración | Actividad | Propósito |
|--------|----------|-----------|-----------|
| 1 | 15 min | Activación: ¿Cómo organizas tus archivos? | Conectar con experiencias previas |
| 2 | 35 min | Teoría: El Sistema de Archivos | Entender el mapa (Windows vs. Linux) |
| 3 | 45 min | Laboratorio 1: Comandos de Navegación | Aprender a moverse (cd, ls, dir, pwd) |
| 4 | 45 min | Laboratorio 2: Comandos de Manipulación | Aprender a crear y modificar (mkdir, touch, cp, mv, rm) |
| 5 | 30 min | Ejercicio Práctico: Estructura de Carpetas | Aplicar comandos en un escenario real |
| 6 | 40 min | Taller Evaluativo: El Desafío del Script | Demostrar maestría en la consola |
| 7 | 10 min | Evaluación y Cierre | Consolidar y recapitular |

---

## 🔄 Activación: El Orden en Tu Mundo (15 min)

### Pregunta de Discusión
Pensa en tu computador personal o en tu celular: 
1. ¿Cómo organizas tus documentos, fotos y música? ¿Usas carpetas? ¿Qué nombres les pones?
2. ¿Alguna vez has "perdido" un archivo y has tenido que buscarlo? ¿Cómo lo hiciste?
3. ¿Qué pasaría si todos los archivos estuvieran en un solo lugar, sin carpetas?

### Analogía de Apertura
El sistema de archivos es como un **archivador gigante con muchísimos cajones y carpetas colgantes**:
- **Disco Duro:** El archivador completo.
- **Carpetas (Directorios):** Los cajones y las carpetas colgantes que agrupan documentos.
- **Archivos:** Los documentos dentro de las carpetas.
- **La Ruta (Path):** La instrucción precisa para encontrar un documento: "Ve al archivador de la esquina, abre el tercer cajón, busca la carpeta 'Impuestos 2024' y saca el archivo 'factura_enero.pdf'".

---

## 🗺️ Teoría: El Sistema de Archivos (35 min)

### Estructura Jerárquica
Todos los sistemas operativos modernos organizan los archivos en una **estructura de árbol invertido**.
- **Raíz (Root):** El punto de partida de todo el sistema.
- **Ramas (Directorios/Carpetas):** Contenedores que pueden tener archivos y otros directorios.
- **Hojas (Archivos):** Donde se almacena la información.

### Analogía Urbana: Medellín como tu Disco Duro

Pensemos en el sistema de archivos como si fuera la ciudad de Medellín. Una dirección completa y única nos lleva a un solo lugar, igual que una ruta nos lleva a un solo archivo.

- **La Raíz (`/` en Linux, `C:\` en Windows):** Es toda la ciudad, **Medellín**. Es el contenedor más grande de todos.
- **Directorios Principales (`/home`, `/etc` o `Program Files`):** Son los grandes **barrios** o **comunas** de la ciudad, como `El Poblado`, `Laureles` o `Belén`.
- **Subdirectorios:** Son unidades más pequeñas dentro de un barrio. Por ejemplo, dentro de `Laureles` (un directorio), podríamos tener una **ciudadela** (`Laureles/CiudadelaPaloGrande`) y dentro de ella, un **edificio** (`Laureles/CiudadelaPaloGrande/Edificio3`).
- **Un Archivo:** Es el **apartamento** específico de alguien, como `Laureles/CiudadelaPaloGrande/Edificio3/Apto501.txt`. Esta es la **ruta absoluta**, la dirección completa que no tiene pérdida.

Y las operaciones que hacemos con los archivos son como las actividades de una ciudad:

- **Crear (`mkdir`, `touch`):** Es como **construir** un nuevo edificio o una nueva casa.
- **Eliminar (`rm`, `rmdir`):** Equivale a **demoler** una construcción. ¡Si demueles un edificio entero (`rm -r`), todo lo que hay adentro se va con él! Por eso es una acción delicada.
- **Mover o Renombrar (`mv`):** Es como si una familia se **trastea** de un apartamento a otro, o si la alcaldía decide **cambiar el nombre de una calle**. La casa sigue siendo la misma, pero su dirección (ruta) cambia.
- **Copiar (`cp`):** Es como hacer una **maqueta idéntica** de una casa y construirla en otro lugar. Ahora tienes dos casas iguales.


### El Mundo Dividido: Windows vs. Linux

#### **En Windows (CMD / PowerShell)**
- **Múltiples Raíces:** No hay una única raíz. Cada unidad de almacenamiento (disco duro, USB, etc.) tiene su propia letra y su propio árbol. `C:\`, `D:\`, etc.
- **Separador:** La barra invertida `\` se usa para separar los directorios.
- **Estructura Típica:**
  ```
  C:\
  ├───Users
  │   └───Jovany
  │       ├───Documents
  │       └───Downloads
  ├───Program Files
  └───Windows
  ```

#### **En Linux (y macOS)**
- **Raíz Única:** Todo comienza en un solo lugar: el directorio raíz `/`.
- **Separador:** La barra normal `/` se usa para separar los directorios.
- **"Todo es un archivo":** Dispositivos, periféricos y conexiones se representan como archivos dentro de esta estructura.
- **Estructura Típica:**
  ```
  /
  ├───home
  │   └───jovany
  │       ├───documentos
  │       └───descargas
  ├───bin  (programas esenciales)
  ├───etc  (archivos de configuración)
  └───var  (archivos variables, como logs)
  ```

---

## 🔬 Laboratorio 1: Comandos de Navegación (45 min)

¡Manos a la obra! Abran su consola. En Windows, busquen "CMD" o "PowerShell". En Linux/macOS, busquen "Terminal".

| Tarea | Comando Linux (Bash) | Comando Windows (CMD/PowerShell) | Descripción |
|---|---|---|---|
| **¿Dónde estoy?** | `pwd` | `cd` (en PowerShell) o `echo %cd%` (en CMD) | **P**rint **W**orking **D**irectory. Muestra la ruta de la carpeta actual. |
| **Ver contenido** | `ls` | `dir` | **L**i**s**t. Lista los archivos y carpetas en el directorio actual. |
| **Cambiar de carpeta** | `cd ruta/a/carpeta` | `cd ruta\a\carpeta` | **C**hange **D**irectory. Nos mueve a otra carpeta. |
| **Ir a la carpeta anterior** | `cd -` | `cd ..` (subir un nivel) | Muy útil para alternar entre dos directorios. |
| **Subir un nivel** | `cd ..` | `cd ..` | Va al directorio "padre". |
| **Ir a tu "casa"** | `cd` o `cd ~` | `cd %USERPROFILE%` | Te lleva a tu carpeta de usuario (`/home/usuario` o `C:\Users\Usuario`). |

### ✨ **Tips de Pro:**
- **Autocompletar con `Tab`:** Escribe las primeras letras de un archivo o carpeta y presiona `Tab`. ¡La consola lo completará por ti! Es el truco más importante.
- **`ls -l` (Linux):** Muestra una lista detallada con permisos, propietario, tamaño y fecha.
- **`ls -a` (Linux):** Muestra todos los archivos, incluyendo los ocultos (los que empiezan con `.`).
- **`dir /A` (Windows):** Muestra todos los archivos, incluyendo los ocultos.

### **Actividad Guiada (20 min):**
1. Abran la terminal.
2. Verifiquen en qué carpeta están.
3. Listen el contenido.
4. Muévanse a su carpeta de Documentos.
5. Creen una carpeta llamada `PruebaSO` (¡oops, aún no hemos visto eso!). Bueno, solo naveguen por las carpetas que ya existen.
6. Vuelvan a su carpeta de inicio (`home`).

---

## 🛠️ Laboratorio 2: Comandos de Manipulación (45 min)

Ahora vamos a crear, mover, copiar y eliminar cosas. **¡CUIDADO! Especialmente con el comando de borrar.**

| Tarea | Comando Linux (Bash) | Comando Windows (CMD/PowerShell) | Descripción |
|---|---|---|---|
| **Crear carpeta** | `mkdir nombre_carpeta` | `mkdir nombre_carpeta` | **M**a**k**e **Dir**ectory. Crea un nuevo directorio. |
| **Crear archivo vacío** | `touch nombre_archivo.txt` | `echo. > nombre_archivo.txt` (CMD) <br> `New-Item nombre_archivo.txt` (PowerShell) | `touch` actualiza la fecha de un archivo, o lo crea si no existe. |
| **Copiar archivo** | `cp origen destino` | `copy origen destino` | Copia un archivo de un lugar a otro. |
| **Mover/Renombrar** | `mv origen destino` | `move origen destino` <br> `ren viejo nuevo` (para renombrar) | Mueve un archivo. Si el destino es un nuevo nombre en la misma carpeta, lo renombra. |
| **Eliminar archivo** | `rm nombre_archivo.txt` | `del nombre_archivo.txt` | **R**e**m**ove. Elimina un archivo. **¡No va a la papelera!** |
| **Eliminar carpeta** | `rmdir nombre_carpeta` <br> `rm -r nombre_carpeta` | `rmdir nombre_carpeta` | `rmdir` solo borra carpetas vacías. `rm -r` borra carpetas con contenido (recursivo). **¡USAR CON MÁXIMO CUIDADO!** |
| **Ver contenido de archivo** | `cat nombre_archivo.txt` | `type nombre_archivo.txt` | Muestra el contenido de un archivo de texto en la consola. |

### **Actividad Guiada (25 min):**
1. Naveguen a su carpeta de Documentos.
2. Creen una carpeta llamada `LaboratorioSO`.
3. Entren en `LaboratorioSO`.
4. Creen un archivo llamado `apuntes.txt`.
5. Creen dos carpetas más: `tareas` y `examenes`.
6. Copien `apuntes.txt` dentro de la carpeta `tareas`.
7. Muevan el `apuntes.txt` original (el que está en `LaboratorioSO`) a la carpeta `examenes`.
8. Renombren el archivo en `examenes` a `examen1.txt`.
9. Listen el contenido de todas las carpetas para verificar.
10. Eliminen el archivo `apuntes.txt` que está en `tareas`.
11. Suban un nivel y eliminen la carpeta `LaboratorioSO` y todo su contenido (`rm -r LaboratorioSO` o `rmdir /S LaboratorioSO`).

---

## 🏗️ Ejercicio Práctico: Estructura de un Proyecto (30 min)

**Misión:** Eres un desarrollador y necesitas crear la estructura de carpetas para un nuevo proyecto web. Usando solo la consola, crea la siguiente estructura dentro de tu carpeta `Documentos`:

```
mi-proyecto-web/
├───assets/
│   ├───images/
│   └───styles/
│       └───main.css
├───src/
│   ├───components/
│   └───app.js
├───index.html
└───README.md
```

**Pasos:**
1. Ve a tu carpeta `Documentos`.
2. Crea la carpeta `mi-proyecto-web` y entra en ella.
3. Crea las carpetas `assets` y `src`.
4. Crea los archivos `index.html` y `README.md`.
5. Entra en `assets` y crea `images` y `styles`.
6. Entra en `styles` y crea `main.css`.
7. Vuelve a la raíz del proyecto, entra en `src` y crea `components` y `app.js`.
8. **¡Reto extra!** Usa el comando `echo "Mi primer proyecto" > README.md` (o `echo "Mi primer proyecto" >> README.md` para añadir sin sobreescribir) para escribir algo en el archivo README. Luego, usa `cat` o `type` para leerlo.

---

## 🏆 Taller Evaluativo: El Desafío del Script (40 min)

**Contexto:** El profesor necesita organizar los trabajos de los estudiantes para tres materias: `Calculo`, `Fisica` y `Algoritmos`. Para cada materia, necesita una carpeta para cada uno de los tres cortes del semestre. Y para cada corte, una carpeta para `Quices` y otra para `Parciales`.

**Tu Tarea:**
1.  **Crea un archivo de texto** llamado `organizar.sh` (para Linux) o `organizar.bat` (para Windows).
2.  **Dentro de ese archivo de texto**, escribe la secuencia de comandos necesarios para crear la siguiente estructura de carpetas:

    ```
    Entregas2025/
    ├───Calculo/
    │   ├───Corte1/
    │   │   ├───Quices/
    │   │   └───Parciales/
    │   ├───Corte2/
    │   │   ├───Quices/
    │   │   └───Parciales/
    │   └───Corte3/
    │       ├───Quices/
    │       └───Parciales/
    ├───Fisica/
    │   ├───(misma estructura que Calculo)
    │   └───...
    └───Algoritmos/
        ├───(misma estructura que Calculo)
        └───...
    ```
3.  **Ejecuta el script:**
    -   En Linux: `bash organizar.sh`
    -   En Windows: `organizar.bat`

**Pista:** ¡No tienes que escribir `mkdir` 50 veces! Puedes crear rutas anidadas. En Linux/PowerShell: `mkdir -p Materia/Corte1/Quices`. En CMD es un poco más manual.

**Evaluación:**
- **Logrado (5.0):** El script crea toda la estructura correctamente con un uso eficiente de los comandos.
- **Bueno (4.0):** El script funciona, pero es repetitivo y poco eficiente.
- **Suficiente (3.0):** Se entrega una lista de comandos que, ejecutados manualmente, crean la estructura.
- **A mejorar (Debajo de 3.0):** La estructura está incompleta o los comandos son incorrectos.

---

## 📝 Evaluación y Cierre (10 min)

### Quiz Rápido
1. ¿Cuál es el comando para ver dónde estás en Linux?
2. ¿Y el comando para listar archivos en Windows?
3. ¿Qué hace `cd ..`?
4. ¿Cuál es la diferencia entre `cp` y `mv`?
5. ¿Por qué `rm -r` es un comando peligroso?

### Reflexión Final
La consola no es "vieja" o "difícil", es **eficiente y poderosa**. Aprender a usarla te da superpoderes para automatizar tareas, gestionar servidores y trabajar mucho más rápido que usando solo la interfaz gráfica. Es el lenguaje universal de los sistemas operativos.

**Frase de cierre:** *"La interfaz gráfica te hace sentir cómodo. La línea de comandos te hace poderoso."*

¡Nos vemos en la siguiente clase, donde instalaremos nuestro primer sistema operativo en una máquina virtual! 🚀

---
**¡Hasta la próxima, comandantes de la terminal!** 💻🔥
