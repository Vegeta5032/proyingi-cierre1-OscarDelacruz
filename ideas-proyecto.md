# Tres ideas de proyecto

**Autor:** Oscar David de la Cruz Alvarado  
**Fecha:** 17 de septiembre de 2026

## Criterios de viabilidad

Consideré que una idea es viable para esta materia si atiende un problema concreto de mi entorno, tiene una parte física fabricable, usa por lo menos un sensor o actuador con un microcontrolador y puede realizarse por principiantes en unas ocho sesiones.

## Idea 1: Contenedor inteligente para avisar cuando está lleno

**Problema.** En los espacios de estudio y convivencia se puede acumular basura cuando el contenedor ya está casi lleno. Esto provoca que las personas dejen residuos fuera o que el personal tenga que revisar varios botes manualmente.

**A quién le pasa.** A los estudiantes, profesores y personal que utilizan los espacios comunes de la IBERO, especialmente cuando hay mucha actividad entre clases.

**Dónde lo he visto.** En los botes de basura de los espacios comunes del campus he observado que, después de los cambios de clase o durante la hora de comida, algunos se llenan rápidamente y quedan residuos alrededor. **Debo confirmar que esta redacción coincida con una observación que yo haya hecho personalmente.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): un sensor ultrasónico mediría la distancia entre la parte superior del bote y la basura para estimar el nivel de llenado; otro sensor podría detectar la mano para abrir la tapa.
- Qué hace con eso (actuador, aviso, pantalla): un servo abriría la tapa sin tocarla y un LED rojo se encendería cuando el nivel llegara a un límite.
- Qué pieza habría que fabricar: una tapa ligera, un soporte para el sensor y una caja protectora para el Arduino y los cables.

## Idea 2: Detector de fugas o derrames de agua

**Problema.** Una pequeña fuga debajo de un lavabo o un derrame que no se atiende pronto puede mojar el piso, desperdiciar agua y causar daños en muebles o instalaciones.

**A quién le pasa.** A las personas que usan baños, cocinas o áreas de servicio en casa y en la escuela, además del personal que tiene que detectar y limpiar el derrame.

**Dónde lo he visto.** En el área del lavabo de mi casa he tenido que revisar si el piso queda húmedo después de usarlo; también he visto que un derrame pequeño puede pasar desapercibido si nadie está cerca. **Debo confirmar que esta redacción describa algo que realmente haya observado.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): un sensor de agua colocado cerca del punto de riesgo detectaría la presencia de humedad.
- Qué hace con eso (actuador, aviso, pantalla): un buzzer y un LED rojo darían una alerta local; opcionalmente se podría agregar una pantalla con el estado del sensor.
- Qué pieza habría que fabricar: una base inclinada para colocar el sensor sin cubrirlo y una carcasa ventilada que proteja el microcontrolador del agua.

## Idea 3: Indicador visual de ruido para salones

**Problema.** Cuando varias personas hablan al mismo tiempo en un salón, el ruido puede aumentar y dificultar que el grupo escuche instrucciones o trabaje con concentración. No siempre se nota el nivel de ruido hasta que ya interrumpió la actividad.

**A quién le pasa.** A estudiantes y profesores que trabajan en salones, laboratorios o espacios de estudio compartidos.

**Dónde lo he visto.** En salones y espacios de trabajo de la universidad he notado que el volumen sube cuando varios equipos conversan a la vez, y que el profesor tiene que pedir silencio repetidamente. **Debo confirmar que esta observación sea propia y modificar el lugar si es necesario.**

**Cómo funcionaría.**
- Qué mide o detecta (sensor): un micrófono analógico mediría la amplitud aproximada del sonido durante intervalos cortos.
- Qué hace con eso (actuador, aviso, pantalla): tres LEDs mostrarían verde, amarillo o rojo según el nivel de ruido, sin grabar conversaciones.
- Qué pieza habría que fabricar: una carcasa de escritorio o pared con una rejilla para el micrófono y una ventana para que se vean los LEDs.

## Tabla de viabilidad

| Criterio | Idea 1 | Idea 2 | Idea 3 |
|---|---|---|---|
| Problema concreto de mi entorno | Sí | Sí | Sí |
| Parte física fabricable | Sí | Sí | Sí |
| Sensor o actuador | Sí | Sí | Sí |
| Construible en ocho sesiones por principiantes | Sí | Sí | Sí |
| Qué tan seguro estoy de lo anterior | Medio | Medio | Medio |

## Mi elección

**Idea elegida:** Indicador visual de ruido para salones.

**Por qué.** Es la idea que considero más viable porque necesita pocos componentes: un micrófono, un microcontrolador y LEDs. También permite construir una carcasa sencilla con impresión 3D o corte láser y probar el sistema en diferentes niveles de sonido. A diferencia de una solución que grabe audio, mi propuesta solo usaría la intensidad aproximada para dar una señal visual y no necesitaría guardar conversaciones.

**Qué todavía no sé.** Todavía necesito comprobar qué sensor de sonido está disponible, calibrar los niveles para que no marque rojo por cualquier ruido y decidir dónde se colocaría sin distraer. También tendría que probar si los LEDs son suficientes o si conviene agregar una pantalla pequeña.

## Declaración de uso de IA

- **Herramienta utilizada:** ChatGPT.
- **Qué le pedí:** ayuda para proponer ideas compatibles con sensores, actuadores, microcontroladores y una pieza fabricable, además de organizar la tabla de viabilidad.
- **Qué modifiqué o rechacé de su respuesta, y por qué:** elegí y adapté las tres ideas, y dejé señaladas las observaciones locales que debo confirmar personalmente. No aceptaré como hecho ninguna observación que no haya visto yo.
