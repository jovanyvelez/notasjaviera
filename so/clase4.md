# 🛠️ Clase 4 (4 horas): Planeación e Instalación de un Sistema Operativo

## "Antes de instalar, hay que pensar: la arquitectura invisible del éxito" 

## 👋 ¡Hola parceros y parceras de Grado Décimo!
Hoy pasamos de la teoría a la planificación estratégica. Aprenderemos **cómo elegir** el sistema operativo adecuado según las necesidades reales de un usuario, equipo o proyecto, y cómo **preparar correctamente el entorno** antes de instalar. También haremos una **simulación guiada paso a paso** del proceso de instalación (ej. Ubuntu y Windows) y revisaremos tareas post-instalación clave.

---

## 🎯 Objetivos de Aprendizaje
Al finalizar esta sesión (240 min) serás capaz de:
- ✅ Identificar criterios técnicos y funcionales para elegir un SO.
- ✅ Analizar requerimientos mínimos vs. recomendados y compatibilidad de hardware.
- ✅ Planificar una instalación segura: respaldo, particiones, modo de arranque.
- ✅ Simular paso a paso una instalación (ej. Ubuntu Desktop / Windows / VM).
- ✅ Comprender tareas post-instalación (drivers, actualizaciones, seguridad básica).
- ✅ Elaborar una matriz de decisión de selección de SO.

---

## 🧭 Ruta de la Clase (Estructura de 4 Horas)
| Bloque | Min | Actividad | Propósito |
|--------|-----|-----------|-----------|
| 1 | 20 | Activación + lectura técnica | Enfocar objetivos de planeación |
| 2 | 35 | Criterios para elegir un SO | Marco de decisión |
| 3 | 30 | Requerimientos y compatibilidad | Evaluar factibilidad |
| 4 | 40 | Simulación Instalación (Parte 1) | Preparación + entorno |
| 5 | 40 | Simulación Instalación (Parte 2) | Ejecución + particiones |
| 6 | 35 | Post-instalación + endurecimiento básico | Operatividad segura |
| 7 | 25 | Taller: Matriz de decisión (grupos) | Aplicación práctica |
| 8 | 15 | Troubleshooting + preguntas | Pensamiento crítico |
| 9 | 10 | Cierre + reflexión + asignación | Consolidación |

---

## 📖 Lectura Técnica Inicial: ¿Por qué Planear?
Instalar un SO sin plan es como montar una ruta en bicicleta sin revisar el clima, el terreno o la condición de la cicla.

### Objetivos de la planeación:
1. Evitar pérdida de datos (respaldo previo).
2. Garantizar compatibilidad (hardware / firmware / drivers).
3. Elegir edición/licencia adecuada (Home, Pro, LTS…).
4. Definir esquema de particiones y sistema de archivos.
5. Optimizar rendimiento vs. recursos disponibles.
6. Reducir riesgos de seguridad iniciales (configuración mínima segura).
7. Estimar tiempo de instalación y ventanas de interrupción (en oficina / laboratorio / colegio).

**Analogía local:** Como planear el montaje de un stand tecnológico en Plaza Mayor: necesitas permisos, energía, espacio, herramientas y plan B.

---

## 🧩 Criterios para Elegir un Sistema Operativo
| Criterio | Pregunta Guía | Impacto |
|----------|---------------|---------|
| Propósito de uso | ¿Ofimática, desarrollo, gaming, servidor, IoT? | Define familia de SO |
| Hardware disponible | ¿CPU, RAM, almacenamiento, GPU? | Afecta rendimiento |
| Licenciamiento / costo | ¿Presupuesto? ¿Open source vs propietario? | Sustentabilidad económica |
| Compatibilidad de software | ¿Requiere apps específicas? | Limita alternativas |
| Seguridad / estabilidad | ¿Necesita alta disponibilidad? | Prioriza LTS / server-oriented |
| Soporte y comunidad | ¿Habrá quien ayude si falla? | Tiempo de respuesta |
| Escalabilidad futura | ¿Crecimiento previsto? | Elección modular |
| Interfaz / usabilidad | ¿Usuarios principiantes o avanzados? | Curva de aprendizaje |
| Gestión remota | ¿Administración centralizada? | Necesita herramientas integradas |
| Energía / movilidad | ¿Portátil, batería limitada? | Optimización energética |

### Ejemplos de Escenarios:
- **Café internet en Envigado:** Windows (software comercial + usuarios variados) o Linux con kiosko para reducción de licencias.
- **Laboratorio de programación:** Linux (Ubuntu LTS) + máquinas virtuales para prácticas.
- **Servidor escolar de plataformas educativas:** Linux Server (estabilidad + costo cero licencias).
- **PC antiguo (2 GB RAM):** Linux ligero (Lubuntu / Xubuntu).
- **Gaming + diseño:** Windows 11 + drivers GPU sobre hardware compatible.
- **IoT prototipos:** Raspberry Pi OS / Ubuntu Server minimal.

---

## 🧪 Requerimientos Mínimos vs Recomendados
| SO | Mínimo Ejemplo | Recomendado | Notas |
|----|----------------|-------------|-------|
| Windows 11 | 4 GB RAM, CPU 2 cores, TPM 2.0, 64 GB disco | 8+ GB RAM, SSD, GPU moderna | Verificar Secure Boot y TPM | 
| Ubuntu 24.04 Desktop | 4 GB RAM, 25 GB disco | 8 GB RAM, 50+ GB, SSD | LTS para estabilidad |
| Linux Mint XFCE | 2 GB RAM, 15 GB disco | 4 GB RAM, 30 GB | Ideal equipos antiguos |
| Android (Emulador) | 8 GB RAM host | 16 GB RAM | Acel. hardware (KVM) |
| FreeRTOS (MCU) | ~64 KB RAM | Según tarea | Requiere toolchain |

### Pasos para verificar:
1. Inventariar hardware (Herramientas: `lshw`, `inxi`, BIOS info, CPU-Z, Speccy).
2. Firmware: ¿BIOS o UEFI? ¿Modo Secure Boot activo?
3. Tabla de compatibilidad: GPU, WiFi, audio, impresoras.
4. Espacio libre: Planificar margen (≥20% libre post-instalación).
5. Periféricos críticos: ¿Drivers disponibles?

---

## 🔐 Consideraciones Previas de Seguridad y Respaldo
| Acción | Herramienta | Motivo |
|-------|-------------|--------|
| Backup de documentos | Disco externo / nube | Evitar pérdida irreversible |
| Verificar integridad ISO | Checksum (SHA256) | Prevenir imágenes corruptas |
| Crear medio booteable | Ventoy / Rufus / balenaEtcher | Arranque confiable |
| Desfragmentar (si HDD previo) | Herramienta SO | Liberar espacio contiguo |
| Anotar contraseñas/licencias | Gestor (Bitwarden) | Restauración posterior |
| Desconectar periféricos innecesarios | — | Reducir fallos de instalación |
| Ajustar orden de arranque | BIOS/UEFI | Boot desde USB correcto |

---

## 💽 Diseño de Particiones (Ej. Dual Boot Ubuntu + Windows)
| Partición | Sistema de Archivos | Tamaño Sugerido | Uso |
|-----------|--------------------|-----------------|-----|
| EFI | FAT32 | 300–500 MB | Arranque (UEFI) |
| Windows (C:) | NTFS | 60–150+ GB | SO + programas |
| Linux Root `/` | ext4 | 30–50 GB | Sistema base |
| Home `/home` | ext4 | Variable (resto) | Datos usuario |
| Swap (si sin zram) | swapfile/partition | 1–2× RAM (máx. 8–16 GB) | Mem virtual |
| Datos compartidos | NTFS/exFAT | Variable | Intercambio entre SO |

**Nota:** En laptops modernos, preferir swapfile y/o zram.

---

## 🌐 Modo de Instalación
| Método | Cuándo Usarlo | Ventajas | Riesgos |
|--------|---------------|----------|--------|
| USB booteable | Instalación física | Rápido | USB corrupto |
| Red (PXE) | Laboratorios | Centralizado | Requiere infra |
| Máquina Virtual | Pruebas / formación | No altera host | Rendimiento menor |
| Contenedor (casos) | Servicios específicos | Ligero | No reemplaza SO completo |

---

## 🖥️ Simulación Paso a Paso: Ubuntu Desktop (Resumen Didáctico)
### Fase 1: Preparación
1. Descargar ISO oficial (ubuntu.com).  
2. Verificar hash SHA256.  
3. Crear USB booteable (balenaEtcher / Ventoy).  
4. Entrar a BIOS/UEFI (F2, DEL, ESC según equipo).  
5. Configurar Boot Priority: USB primero.  

### Fase 2: Arranque e Inicio
6. Seleccionar "Try or Install Ubuntu".  
7. Comprobar WiFi (si se requiere).  
8. Probar compatibilidad (touchpad, sonido, pantalla).  

### Fase 3: Instalación
9. Elegir idioma y layout del teclado.  
10. Tipo de instalación: Normal / Minimal (según uso).  
11. Opciones adicionales: Descargar updates + instalar software de terceros (drivers).  
12. Particionado: Manual (para dual boot) o automático (único SO).  
13. Configurar zona horaria (Bogotá).  
14. Crear usuario, hostname y contraseña segura.  

### Fase 4: Proceso y Finalización
15. Copia de archivos e instalación de paquetes.  
16. Instalador del bootloader GRUB (si dual boot).  
17. Reinicio y retiro del USB.  
18. Primer login: revisar actualizaciones (`Software Updater` o `sudo apt update && sudo apt upgrade`).  

### Fase 5: Post-Instalación Básica
19. Instalar codecs / utilidades (según necesidad).  
20. Verificar drivers propietarios (NVIDIA).  
21. Crear snapshot inicial (Timeshift / BTRFS).  
22. Configurar firewall (`ufw enable`).  
23. Crear cuentas adicionales (si laboratorio).  
24. Instalar herramientas (VS Code, navegadores, Docker según rol).  

---

## 🪟 Simulación Paso a Paso: Windows 11 (Resumen)
1. Descargar ISO oficial (Microsoft).  
2. Crear USB (Rufus, Modo GPT + UEFI).  
3. Boot desde USB → Seleccionar idioma / región.  
4. "Install Now" → Licencia (clave o continuar).  
5. Elegir edición (si aplica).  
6. Tipo de instalación: Custom para particionar.  
7. Eliminar particiones antiguas (solo si reemplazo total) o seleccionar espacio libre.  
8. Crear particiones automáticas (Windows genera EFI + MSR + primaria).  
9. Formatear partición primaria (NTFS).  
10. Copia de archivos + reinicios.  
11. OOBE (Out Of Box Experience): Región, teclado, red, cuenta Microsoft / local, privacidad.  
12. Actualizaciones iniciales (Windows Update).  
13. Instalar drivers (chipset, GPU, WiFi si faltan).  
14. Configurar antivirus / Defender políticas.  
15. Instalar apps de productividad (Office / LibreOffice / navegadores).  

---

## 🔄 Virtualización vs Instalación Física
| Aspecto | Virtualización | Física |
|---------|----------------|-------|
| Riesgo de datos | Bajo (aislado) | Alto si mal planificado |
| Rendimiento | Limitado (depende host) | Óptimo |
| Pruebas múltiples | Fácil (snapshots) | Lento (reinstalar) |
| Acceso hardware directo | Limitado (GPU passthrough complejo) | Completo |
| Uso educativo | Ideal para ensayo | Ideal para práctica final |

---

## 🧪 Actividad 1: Checklist de Pre-Instalación (15 min)
En parejas, elaborar una lista realista para un PC del laboratorio:
- Hardware detectado (CPU, RAM, disco, firmware).  
- Tipo de instalación (dual boot, reemplazo, VM).  
- Particiones planificadas.  
- Riesgos identificados + mitigación (ej. backup).  
- SO elegido y por qué.  

Compartir 2 hallazgos comunes con el grupo.

---

## 📊 Actividad 2: Matriz de Decisión (Grupos de 3) (25 min)
| Criterio | Peso (1–5) | Windows 11 | Ubuntu LTS | Linux Mint | Resultado |
|----------|------------|------------|-----------|-----------|-----------|
| Compatibilidad software | 5 | | | | |
| Requerimientos hardware | 4 | | | | |
| Costo licencias | 5 | | | | |
| Soporte comunitario | 3 | | | | |
| Seguridad / estabilidad | 4 | | | | |
| Curva aprendizaje | 3 | | | | |
| Mantenimiento | 2 | | | | |
| TOTAL | — | | | | |

Cada grupo pondera y expone su decisión (3 min). Comparar divergencias.

---

## 🖱️ Actividad 3: Simulación Guiada (30–40 min)
El docente proyecta (o usa VM) el proceso (Ubuntu o Windows). Estudiantes registran en una plantilla:
| Paso | Captura / Descripción | Riesgo Potencial | Nota |
|------|-----------------------|------------------|------|
| 1 | Selección de idioma | Escoger mal → configuración teclado | |
| … | … | … | … |

Al final, cada estudiante marca 3 puntos críticos y explica por qué.

---

## 🛡️ Post-Instalación (Hardening Básico)
| Acción | SO | Herramientas | Objetivo |
|--------|----|-------------|----------|
| Actualizaciones | Ambos | Windows Update / apt | Parchear vulnerabilidades |
| Firewall | Ambos | Defender / ufw | Reducir superficie |
| Usuarios y roles | Ambos | MMC / `adduser` | Menos privilegios |
| Copias de seguridad | Ambos | Historial archivos / Timeshift | Recuperación |
| Antivirus / Anti-malware | Windows | Defender | Protección inicial |
| Limpiar bloatware | Windows | Winget / panel | Optimizar |
| Repositorios confiables | Linux | apt sources | Integridad |
| Snapshots (VM) | VM | VirtualBox / VMWare | Rollback |

---

## 🚨 Troubleshooting Rápido (Escenarios)
| Problema | Causa Probable | Solución |
|----------|----------------|----------|
| No detecta USB booteable | Modo Legacy vs UEFI | Rehacer USB GPT + UEFI |
| Pantalla negra post-install | Driver GPU | Modo recovery / instalar driver | 
| No WiFi en Linux | Firmware faltante | Instalar paquete `linux-firmware` |
| Boot salta a Windows | GRUB no instalado | Reparar con live USB (update-grub) |
| Error de disco lleno | Partición insuficiente | Redimensionar / limpiar |

---

## 🧠 Preguntas Reflexivas
1. ¿Qué pesa más: compatibilidad o costo en un colegio público?  
2. ¿Cuándo usarías una VM antes de formatear?  
3. ¿Por qué validar hashes de una ISO?  
4. ¿Qué impacto ecológico tiene prolongar la vida útil con un SO ligero?  
5. ¿Cómo reduce riesgos un buen esquema de particiones?  

---

## 📝 Mini Quiz (Opcional – 8 Min)
1. Define "requerimiento mínimo".  
2. Diferencia BIOS vs UEFI (1 idea clave).  
3. ¿Qué es una partición EFI?  
4. Nombra 2 acciones post-instalación esenciales.  
5. ¿Por qué crear respaldo antes de formatear?  

Respuestas guía: 1. Configuración mínima para ejecutar. 2. UEFI soporta interfaces modernas y GPT vs BIOS legado. 3. Partición para cargadores de arranque en sistemas UEFI. 4. Actualizar + configurar firewall. 5. Evitar pérdida de datos.

---

## 🗂️ Entregables de la Clase
| Entregable | Formato | Evaluación |
|------------|---------|-----------|
| Checklist pre-instalación | Hoja / digital | Compleción y pertinencia |
| Matriz de decisión | Tabla | Justificación + pesos |
| Plantilla simulación | Registro | Identificación de riesgos |

---

## 🏆 Evaluación
| Componente | Peso |
|------------|------|
| Participación activa | 20% |
| Matriz de decisión | 30% |
| Registro simulación | 25% |
| Checklist + reflexión | 15% |
| Quiz / preguntas | 10% |

Rubrica simplificada (ejemplo Matriz):
- 5: Criterios justificados con datos reales
- 4: Justificaciones claras, leves omisiones
- 3: Generalidades sin datos
- 2: Inconsistente
- 1: Incompleto

---

## 🔭 Proyecto para Casa
**"Plan de Migración Sostenible"**: Elegir un computador viejo del barrio o familia y proponer plan de migración a un SO ligero (diagnóstico hardware, elección, riesgos, plan de respaldo, pasos). Entrega: 1 página.

---

## 💡 Tips Clave
- Siempre verifica la etiqueta del disco antes de particionar.
- No instales software masivo antes de actualizar el sistema.
- Usa cuentas separadas para administración y uso diario.
- Documenta cada cambio (especialmente en laboratorios educativos).

---

## 🌟 Cierre y Reflexión Final
Planear correctamente ahorra tiempo, previene pérdidas y asegura que la tecnología sirva a las personas. La instalación no es solo un proceso técnico: es una **decisión estratégica** alineada con necesidades reales.

Frase de cierre: *"La preparación convierte la instalación en un acto de precisión, no de improvisación".*

¡Nos vemos en la próxima clase! 🔐🌀 (Seguridad, usuarios y políticas avanzadas).

---

**Fin de la Clase 4**
