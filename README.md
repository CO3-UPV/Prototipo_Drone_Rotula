## Cambio de firmware
Todo lo referido al cambio de firmware esta en la carpeta ConfigESC.

ESC tienen una etiqueta con la descripción de RC INNOVATIONS  30A OPTO Small 2-6LiPo/600Hz y en la pagina web los puedes encontrar como RCI Spider 30A OPTO "Small". Este ESC es un rebrand del ZTW Spider 30A OPTO Small. Viene flasheado con SimonK. Con un firmware desconocido y pone 600 Hz, he estado probando los diferentes entradas y no acabo de entender como funcionan. 

Contexto: Los ESCs llevan un microcontrolador (MCU) intenamente, pues el MCU que lleva este ESC es de 8 bits, es por eso que BLHeliSuite16714903 es la última version compatible con este tipo de MCUs.

Al final me decidi por modificar el firmware de fabrica por uno más que conocido como es BLHeli con el programa BLHeliSuite16714903, solo disponible para Windows. El firmware que he elegido según la documentación es Blue Series 30A ESC MULTI, la documentación la puedes encontrar en el propio programa en la pestaña de BLHeli info -> Manuals. Aquí tienes un video de como flashear este firmware con un Arduino (Uno, Nano, etc): https://www.youtube.com/watch?v=i6lhMcQLRSU (también hay un backup en el repo)

Nota: El arduino Nano y Uno son el mismo con distinto formato de PCB, es decir, la forma de la tarjeta y los pines.

## Notas sobre el prototipo
El prototipo V2 ya es funcional con el código de Simulink para Arduino Due, por tanto, habrá que hacer una iteración del mismo para incluir más especificaciones de cara a una nueva versión de este. El formato del prototipo sería similar con modificaciones del mismo. Quizás añadir una IMU para hacer más completo el prototipo.

En la carpeta CADs puedes encontrar el SOLIDWORKS actual.
En la carpeta SimulinkCode puedes encontrar un ejemplo del control del drone para los potenciometros. 

### Ideas para el siguiente
Para la siguiente versión necesitamos un Slip Ring para los cables
- 4x3 cables para los ESCs
- 4 cables para la IMU
- 2+2 cables para los potenciometros (Opcional)
Es una idea sólo, hay otras formas de hacerlo.
