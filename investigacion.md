# Investigación: ¿esto ya existe? ¿quién lo dice?

**Autor:** Oscar David de la Cruz Alvarado<br>
**Fecha:** 20 de septiembre de 2026<br>
**Ideas analizadas:** ver [[ideas-proyecto]] o [ideas-proyecto.md](ideas-proyecto.md)

## Parte 1. Un ejemplo que ya existe, por cada idea

### Idea 1: Lentes básicos de asistencia para personas ciegas

- **Qué encontré:** [Blind Glass for Visually Impaired Using Audio](https://www.electronicwings.com/users/NeerajaA/projects/6691/blind-glass-for-visually-impaired-using-audio), un proyecto de ElectronicWings.
- **Enlace:** [ElectronicWings: blind glass for visually impaired](https://www.electronicwings.com/users/NeerajaA/projects/6691/blind-glass-for-visually-impaired-using-audio).
- **Qué hace:** conecta un sensor ultrasónico a un Arduino Nano para detectar obstáculos y proporciona una alerta de audio para apoyar el desplazamiento de una persona con discapacidad visual.
- **Qué aprendí:** el proyecto muestra una arquitectura parecida a la que quiero estudiar, pero tendría que validar por mi cuenta la comodidad, el alcance y la seguridad del prototipo.
- **Por qué no resuelve mi caso:** es un proyecto educativo general y no está diseñado para las medidas, comodidad ni espacios específicos donde yo lo probaría. Mi propuesta sería un prototipo más básico, con vibración graduada, una carcasa ligera y pruebas controladas; no lo presentaría como reemplazo del bastón ni como dispositivo médico.

### Idea 2: Aviso de comida lista en la cafetería de la IBERO

- **Qué encontré:** [Square QR code ordering](https://squareup.com/us/en/online-ordering/qr-code-ordering), un sistema comercial en el que el cliente escanea un código QR, ordena desde el celular y el pedido llega al sistema del negocio.
- **Enlace:** [Square: QR code ordering for restaurants](https://squareup.com/us/en/online-ordering/qr-code-ordering).
- **Qué hace:** relaciona códigos QR con lugares de pedido, envía la orden al sistema del negocio y permite avisar al cliente mediante actualizaciones de estado. La documentación de Square también explica que se pueden enviar avisos cuando el pedido está listo para recoger.
- **Por qué no resuelve mi caso:** es un servicio comercial que depende de la configuración y el costo de Square. No está adaptado al menú, flujo de trabajo ni sistema de la cafetería de la IBERO. Mi primera versión usaría pedidos simulados, un identificador y un tablero sencillo para probar el proceso antes de proponer una integración real.

### Idea 3: Software de análisis y backtesting para trading

- **Qué encontré:** [Backtrader](https://www.backtrader.com/), un framework de Python para crear estrategias, cargar datos históricos, ejecutar backtesting y analizar resultados.
- **Enlace:** [Documentación de Backtrader](https://www.backtrader.com/docu/).
- **Qué hace:** permite definir una estrategia, agregar indicadores y datos, ejecutar un motor de backtesting y analizar las operaciones. También tiene documentación sobre fuentes de datos y brokers.
- **Por qué no resuelve mi caso:** es un framework y no una aplicación completa con la interfaz, reglas de riesgo y flujo de trabajo que yo quiero. Además, que una estrategia tenga buenos resultados históricos no garantiza que funcione en el futuro. Mi proyecto tendría que comenzar con backtesting y paper trading, sin operar dinero real automáticamente.

## Parte 2. Fuentes de la idea que elegí

### Fuente 1

| Campo | Contenido |
|---|---|
| Autor u organización | Organización Mundial de la Salud (OMS) |
| Título | Assistive technology |
| Año | 2024 |
| Enlace | [OMS: Assistive technology](https://www.who.int/news-room/fact-sheets/detail/assistive-technology) |
| Tipo | Sitio institucional / ficha informativa |
| Por qué le creo | La OMS es una organización internacional especializada en salud y accesibilidad. La fuente explica qué es la tecnología de asistencia y cómo puede apoyar la movilidad y la visión. |
| Qué dato me dio | La tecnología de asistencia incluye productos físicos como lentes y bastones, y puede ayudar a mantener o mejorar la movilidad, la visión, la autonomía y la inclusión. |

### Fuente 2

| Campo | Contenido |
|---|---|
| Autor u organización | ElectronicWings / NeerajaA |
| Título | Blind Glass for Visually Impaired Using Audio |
| Año | s. f. |
| Enlace | [ElectronicWings: blind glass for visually impaired](https://www.electronicwings.com/users/NeerajaA/projects/6691/blind-glass-for-visually-impaired-using-audio) |
| Tipo | Proyecto/tutorial de electrónica |
| Por qué le creo | La página identifica el proyecto, describe sus componentes y explica cómo se usa el sensor ultrasónico con un microcontrolador. La tomaría como referencia inicial, pero no como una validación clínica o de seguridad. |
| Qué dato me dio | Es posible combinar un Arduino Nano, un sensor ultrasónico y una alerta de audio en un prototipo portátil; yo estudiaría cambiar parte del aviso por vibración. |

### Fuente 3

| Campo | Contenido |
|---|---|
| Autor u organización | Arduino Project Hub |
| Título | How Does an Ultrasonic Sensor Really Work? |
| Año | 2026 |
| Enlace | [Arduino Project Hub: ultrasonic sensor](https://projecthub.arduino.cc/shmuel_rubin/how-does-an-ultrasonic-sensor-really-work-e66c78) |
| Tipo | Tutorial técnico |
| Por qué le creo | El tutorial muestra el sensor HC-SR04, su conexión y un ejemplo de código. Lo usaría para entender el funcionamiento electrónico, pero tendría que comprobar los valores con el sensor real y no asumir que el tutorial garantiza el resultado final. |
| Qué dato me dio | El microcontrolador activa el pin de disparo, mide el tiempo del eco y usa ese tiempo para estimar la distancia al objeto. |

## Parte 3. Qué haría distinto

Mi propuesta tomaría la idea básica de detectar obstáculos, pero la limitaría a un prototipo sencillo y económico para aprender. Usaría uno o dos sensores ultrasónicos montados en una estructura ligera, un motor vibrador y una señal que aumente su frecuencia cuando el obstáculo esté más cerca. Preferiría la vibración para no bloquear la audición de la persona. También dejaría claro que sería una ayuda adicional y no un reemplazo del bastón, del perro guía o de una evaluación profesional. Antes de probarlo con una persona, tendría que hacer pruebas controladas y pedir autorización.

## Parte 4. Qué me falta averiguar

- [ ] Qué sensor ultrasónico es suficientemente pequeño, ligero y confiable para montarlo en los lentes.
- [ ] Qué distancia mínima y máxima debe detectar el prototipo para que la alerta sea útil.
- [ ] Cómo distribuir el peso de la batería y el microcontrolador sin que los lentes sean incómodos.
- [ ] Cómo hacer pruebas seguras, con autorización y sin presentar el prototipo como un dispositivo médico.

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT.
- **Qué le pedí:** apoyo para encontrar ejemplos existentes de las tres ideas, organizar fuentes y redactar la comparación con mi propuesta.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** seleccioné la idea de los lentes como la principal, revisé los enlaces y adapté la propuesta para que sea un prototipo básico de asistencia. También limité el alcance: no afirmo que los lentes eviten todos los accidentes ni que sustituyan herramientas profesionales de movilidad.
