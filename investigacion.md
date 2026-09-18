# Investigación: ¿esto ya existe? ¿quién lo dice?

**Autor:** Oscar David de la Cruz Alvarado  
**Fecha:** 17 de septiembre de 2026  
**Ideas analizadas:** ver [ideas-proyecto.md](ideas-proyecto.md) o [[ideas-proyecto]].

## Parte 1. Un ejemplo que ya existe, por cada idea

### Idea 1: Contenedor inteligente para avisar cuando está lleno

- **Qué encontré:** [Smart Dustbin with Garbage Level Monitoring](https://projecthub.arduino.cc/msr048/37e1cbce-2fc1-4edb-8d5b-888029c6a54c), un proyecto publicado en Arduino Project Hub.
- **Enlace:** [Abrir el proyecto de Arduino Project Hub](https://projecthub.arduino.cc/msr048/37e1cbce-2fc1-4edb-8d5b-888029c6a54c).
- **Qué hace:** usa sensores ultrasónicos para revisar el nivel de basura y un servo para mover la tapa; también muestra el estado con LEDs y una pantalla.
- **Por qué no resuelve mi caso:** es un proyecto de referencia y no está adaptado al tamaño, ubicación ni forma de mantenimiento de los botes que yo usaría en mi entorno. Mi primera versión sería más sencilla y solo daría una alerta local.

### Idea 2: Detector de fugas o derrames de agua

- **Qué encontré:** [Water Leakage Detection System](https://projecthub.arduino.cc/aanchal0431/water-leakage-detection-system-5e94f2), un sistema con sensor de agua, buzzer y conexión a la nube.
- **Enlace:** [Abrir el proyecto de Arduino Project Hub](https://projecthub.arduino.cc/aanchal0431/water-leakage-detection-system-5e94f2).
- **Qué hace:** detecta agua, activa una alarma y registra información adicional de temperatura y humedad; el proyecto también contempla enviar datos a un servicio en la nube.
- **Por qué no resuelve mi caso:** para un primer prototipo tendría demasiados componentes y dependería de conexión de red. Mi propuesta se enfocaría en una alerta inmediata y local, con menos piezas.

### Idea 3: Indicador visual de ruido para salones

- **Qué encontré:** [Hear the Light: LED Sound Level Meter](https://projecthub.arduino.cc/greenvariable/hear-the-light-led-sound-level-meter-7d3ca6), un medidor que usa un micrófono y una serie de LEDs para representar la intensidad del sonido.
- **Enlace:** [Abrir el proyecto de Arduino Project Hub](https://projecthub.arduino.cc/greenvariable/hear-the-light-led-sound-level-meter-7d3ca6).
- **Qué hace:** toma varias lecturas del micrófono, calcula una diferencia entre el valor máximo y mínimo y enciende una cantidad de LEDs de acuerdo con el nivel detectado.
- **Por qué no resuelve mi caso:** el ejemplo usa más LEDs y un registro de desplazamiento, mientras que mi primer prototipo tendría tres estados y una carcasa pensada para un salón. Además, tendría que calibrarlo en el lugar donde se usaría.

## Parte 2. Fuentes de la idea que elegí

### Fuente 1

| Campo | Contenido |
|---|---|
| Autor u organización | GreenVariable, publicado en Arduino Project Hub |
| Título | Hear the Light: LED Sound Level Meter |
| Año | 2024 |
| Enlace | [Arduino Project Hub](https://projecthub.arduino.cc/greenvariable/hear-the-light-led-sound-level-meter-7d3ca6) |
| Tipo | Proyecto técnico/tutorial |
| Por qué le creo | Muestra los componentes, el código y la forma general de tomar las lecturas; aun así, tendría que probar y calibrar el circuito por mi cuenta. |
| Qué dato me dio | Se puede estimar un nivel de sonido con lecturas del micrófono y representar el resultado con varios LEDs. |

### Fuente 2

| Campo | Contenido |
|---|---|
| Autor u organización | Arduino |
| Título | Arduino Nano 33 BLE — Datasheet, ejemplo de aplicación “Sound spectrum” |
| Año | 2026 |
| Enlace | [Documentación técnica de Arduino](https://docs.arduino.cc/resources/datasheets/ABX00030-datasheet.pdf) |
| Tipo | Documentación técnica del fabricante |
| Por qué le creo | Es documentación del fabricante de una tarjeta y describe sus capacidades de hardware; es una fuente más confiable para conocer la placa que un tutorial sin autor identificado. |
| Qué dato me dio | Arduino presenta el análisis de sonido como una aplicación posible al conectar una tarjeta con un micrófono o amplificador. |

### Fuente 3

| Campo | Contenido |
|---|---|
| Autor u organización | Arduino |
| Título | Arduino Language Reference |
| Año | s. f. |
| Enlace | [Referencia del lenguaje de Arduino](https://docs.arduino.cc/language-reference/) |
| Tipo | Documentación técnica oficial |
| Por qué le creo | Es la referencia oficial de las funciones del lenguaje que usaría para leer entradas y controlar salidas; la consultaría junto con pruebas del circuito. |
| Qué dato me dio | La referencia incluye funciones como `analogRead()`, `digitalWrite()` y `millis()`, que pueden servir para leer el micrófono y controlar los LEDs sin bloquear todo el programa. |

## Parte 3. Qué haría distinto

Mi propuesta sería más sencilla que el medidor de sonido que encontré: usaría únicamente tres LEDs para comunicar un estado fácil de entender. La carcasa estaría pensada para colocarse en un salón y protegería el circuito sin tapar el micrófono. No grabaría audio ni enviaría conversaciones a internet; solo procesaría localmente la intensidad aproximada del sonido. También tendría que calibrar los límites en el lugar real, porque el mismo valor puede sentirse diferente en un salón vacío o en uno con muchas personas.

## Parte 4. Qué me falta averiguar

- [ ] Qué módulo de micrófono y qué microcontrolador están disponibles para el equipo.
- [ ] Qué valores produce el sensor en silencio, conversación normal y ruido alto.
- [ ] Si tres LEDs son suficientes o si una pantalla haría más claro el resultado.
- [ ] Confirmar en qué salón o espacio podría probarse el prototipo.

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT.
- **Qué le pedí:** apoyo para organizar la investigación y encontrar ejemplos de proyectos parecidos con enlaces verificables.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** revisé los enlaces, seleccioné la idea que considero más viable y escribí con mis palabras por qué cada ejemplo no resuelve exactamente mi caso. Antes de entregar volveré a abrir cada enlace y corregiré cualquier dato que no pueda comprobar.
