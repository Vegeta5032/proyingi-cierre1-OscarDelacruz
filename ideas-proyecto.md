# Tres ideas de proyecto

**Autor:** Oscar David de la Cruz Alvarado  
**Fecha:** 17 de septiembre de 2026

## Criterios de viabilidad

Consideré que una idea es viable para esta materia si atiende un problema concreto de mi entorno, tiene una parte física fabricable, usa por lo menos un sensor o actuador con un microcontrolador y puede realizarse por principiantes en unas ocho sesiones. En la idea del software de trading, la parte física podría ser una estación o módulo de señal; el software completo quedaría como una versión inicial y limitada.

## Idea 1: Lentes básicos de asistencia para personas ciegas

**Problema.** Una persona ciega puede encontrar obstáculos a la altura del torso o de la cabeza que no siempre detecta con un bastón. Chocarse con esos objetos puede causar golpes, caídas o inseguridad al caminar.

**A quién le pasa.** A personas ciegas o con discapacidad visual que caminan en espacios interiores o exteriores con obstáculos inesperados. La intención es que sea una ayuda adicional y no un reemplazo del bastón, del perro guía o de otras herramientas de movilidad.

**Dónde lo he visto.** He pensado en este problema al observar que en pasillos, salones y espacios concurridos puede haber personas, mochilas, puertas abiertas u objetos a diferentes alturas. **Debo cambiar esta frase por un lugar y una situación que yo haya observado personalmente antes de entregar.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): uno o dos sensores ultrasónicos medirían la distancia aproximada hacia los obstáculos que estén enfrente.
- Qué hace con eso (actuador, aviso, pantalla): un buzzer o un pequeño motor vibrador avisaría con pulsos más rápidos cuando el obstáculo esté más cerca. El prototipo no necesitaría cámara ni reconocimiento facial.
- Qué pieza habría que fabricar: una montura de lentes o una pieza frontal ligera para sostener el sensor, además de una caja pequeña para el microcontrolador y la batería.

**Por qué me interesa.** Esta es mi idea principal porque me gustaría desarrollar algo que pueda ayudar a las personas y que tenga un propósito social. Los lentes serían básicos, económicos y enfocados en detectar obstáculos; no intentarían resolver toda la movilidad de una persona.

## Idea 2: Aviso de comida lista en la cafetería de la IBERO

**Problema.** Cuando un estudiante pide comida en la cafetería, puede tener que esperar cerca del mostrador o regresar varias veces para preguntar si su pedido ya está listo. Esto genera filas, pérdida de tiempo y concentración de personas en el mismo lugar.

**A quién le pasa.** A los estudiantes, profesores y trabajadores que compran comida en la cafetería de la IBERO, especialmente durante los horarios de mayor demanda.

**Dónde lo he visto.** En la cafetería de la IBERO he observado que las personas esperan cerca del área de entrega y preguntan si ya está listo su pedido. **Debo confirmar el lugar y describir una situación específica que yo haya visto personalmente.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): el usuario escanearía un código QR en la cafetería y el sistema registraría un identificador del pedido; el personal podría actualizar el estado desde una pantalla sencilla.
- Qué hace con eso (actuador, aviso, pantalla): al estar listo el pedido, la aplicación o una página móvil enviaría una notificación al celular indicando que ya puede recogerse. La primera versión podría usar un código de pedido y un tablero para el personal.
- Qué pieza habría que fabricar: una base o letrero físico con el código QR, y posiblemente una pequeña pantalla o indicador en el área de entrega.

**Por qué me interesa.** Esta idea ayudaría a la comunidad de la escuela porque reduciría esperas innecesarias y haría más ordenado el proceso de entrega. También se podría probar primero con un menú y pedidos simulados, sin modificar todavía el sistema real de la cafetería.

## Idea 3: Software de análisis y backtesting para trading

**Problema.** Una persona que hace trading puede tardar mucho en comparar estrategias, revisar datos históricos y vigilar varios mercados. También puede tomar decisiones impulsivas si opera sin reglas claras o sin haber probado antes una estrategia.

**A quién le pasa.** A personas que hacen trading o que están aprendiendo a operar en mercados de criptomonedas, acciones y forex, y que necesitan analizar sus estrategias de una forma más ordenada.

**Dónde lo he visto.** En mi propia experiencia haciendo trading he tenido que revisar gráficas, comparar movimientos y pensar qué habría pasado si hubiera aplicado una estrategia en otro momento. **Debo agregar una situación concreta y personal que pueda explicar con honestidad.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): en este caso el equivalente a la entrada sería el precio histórico y los indicadores técnicos descargados de una fuente de datos; no usaría sensores físicos para tomar decisiones financieras.
- Qué hace con eso (actuador, aviso, pantalla): el software ejecutaría backtesting, mostraría resultados como rendimiento, pérdidas, operaciones y retrocesos, y generaría señales. Como primera versión solo trabajaría con datos históricos y paper trading; no operaría dinero real de forma autónoma.
- Qué pieza habría que fabricar: una estación o carcasa física sencilla con indicadores LED para mostrar si el sistema está ejecutando una prueba, si terminó o si requiere atención. La parte principal sería de software.

**Por qué me interesa.** Me gusta el trading y ya tengo interés en aprender más sobre los mercados, pero creo que me iría mejor si desarrollo una herramienta que me obligue a probar las estrategias con datos antes de tomar decisiones. Una versión futura podría conectarse a una cuenta de práctica; operar dinero real requeriría más pruebas, controles de seguridad y supervisión humana.

## Tabla de viabilidad

| Criterio | Idea 1: lentes | Idea 2: cafetería | Idea 3: trading |
|---|---|---|---|
| Problema concreto de mi entorno | Sí | Sí | Parcial |
| Parte física fabricable | Sí | Sí | Parcial |
| Sensor o actuador | Sí | Sí | Parcial |
| Construible en ocho sesiones por principiantes | Sí | Parcial | No |
| Qué tan seguro estoy de lo anterior | Medio | Medio | Bajo |

## Mi elección

**Idea elegida:** Lentes básicos de asistencia para personas ciegas.

**Por qué.** Es la idea que más me interesa porque tiene un beneficio social directo: ayudar a que una persona ciega detecte obstáculos que podrían estar fuera del alcance del bastón. También tiene una relación clara entre sensor, microcontrolador, aviso y pieza fabricable. El alcance se puede mantener pequeño usando solo medición de distancia y vibración, por lo que es más realista para un equipo principiante que un sistema completo de trading.

**Qué todavía no sé.** Necesito investigar qué sensor ultrasónico tiene el tamaño y consumo adecuados, cómo colocar los sensores sin hacer incómodos los lentes y cómo calibrar las alertas. También tendría que probar el prototipo de manera segura y con autorización, sin presentarlo como un dispositivo médico ni como un sistema que garantice evitar todos los obstáculos.

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT.
- **Qué le pedí:** ayuda para organizar tres ideas relacionadas con asistencia a personas ciegas, servicio de cafetería y trading, incluyendo sensores, actuadores, software y viabilidad.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** elegí las ideas que realmente me interesan, cambié el enfoque de la tercera para que el primer prototipo sea de backtesting y paper trading, y debo reemplazar las frases marcadas con mis observaciones personales. No presentaré la operación autónoma con dinero real como una función ya construida.
