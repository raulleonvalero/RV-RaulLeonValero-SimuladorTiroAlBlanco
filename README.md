# 🎯 Simulador de Tiro al Blanco en Realidad Virtual (Unreal Engine)

## 📄 Documentación
### 🕹️ Descripción de la experiencia
Juego de realidad virtual desarrollado en Unreal Engine para la Universidad de Alicante, 
donde tomas el control de un vaquero y debes demostrar tu puntería usando hachas y revólveres para acertar en objetivos. 
Una experiencia inmersiva que combina acción y precisión en un entorno del Viejo Oeste.

## 🎮 ¿Cómo jugar?
Comienzas en una sala con un mensaje explicativo que se resume en avanzar a la zona de disparo,
en esta zona deberas tocar la campana (situada a la izquierda y de color amarillo)
con la tecla p en ordenador y con el boton B en las metaquest.
Después aparecerán objetos cerca de la campana que podrás coger y utilizar para lanzar a los muñecos,
ratas, patos y lingote de oro que estan situados en la zona de disparo, cuando termines los objetos
tienes que pulsar la campana para subir la puntuación al ranking y generar nuevos objetos y una nueva ronda.
### 🎛️ Controles
**Ordenador**

P ➡ Para tocar la campana al colisionar la mano con ella

W ➡ Moverse hacia delante

S ➡ Moverse hacia atras

D ➡ Moverse hacia el lado derecho

A ➡ Moverse hacia el lado izquierdo

Q ➡ Moverse hacia arriba

E ➡ Moverse hacia abajo

Raton ➡ Rotar camara 

R ➡ Coger objeto con la izquierda

T ➡ Coger objeto con la derecha

Y ➡ Lanzar objeto con la izquierda

U ➡ Lanzar objeto con la derecha

L pressed ➡ Te teletransporta hacia donde apuntes

L hold and released ➡ Activa y desactiva el dibujado del teletransporte,  
este sigue funcionando pero no se vera donde apuntas

![CONTROLESteclado](https://github.com/user-attachments/assets/c81d9b3b-d9eb-4cec-9eba-a9c74c5fe9ac)


**Metaquest**

B ➡ Para tocar la campana al colisionar la mano con ella

Y pressed ➡ Te teletransporta hacia donde apuntes

Y hold and released ➡ Activa y desactiva el dibujado del teletransporte,  
este sigue funcionando pero no se vera donde apuntas

Gatillo izquierdo ➡ Coger objeto con la izquierda

Gatillo derecho ➡ Coger objeto con la derecha

X ➡ Lanzar objeto con la izquierda

A ➡ Lanzar objeto con la derecha

![controles2](https://github.com/user-attachments/assets/22df3edf-3821-4dae-a812-5c4c3763e262)


## Licencias
### 📜 Licencias de sonidos
Los sonidos utilizados en el proyecto pertenecen a estas licencias y estan ubicadas en estas carpetas dentro del repositorio

Project/Content/ModelosPropios/sonidos/404238__rafash1306__graznido-2.uasset
Version/formato original: 404238__rafash1306__graznido-2.wav  
by [rafash1306] is licensed under CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/)

Project/Content/ModelosPropios/sonidos/317663__peacewaves__talking_rat.uasset
Version/formato original: 317663__peacewaves__talking_rat.wav 
by [Peacewaves] is licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/)

Project/Content/ModelosPropios/sonidos/472399__joseagudelo__16_raton_chillando.uasset
Version/formato original: 472399__joseagudelo__16_raton_chillando.wav 
by [JoseAgudelo] is licensed under CC BY 1.0 (https://creativecommons.org/publicdomain/zero/1.0/)

Project/Content/ModelosPropios/sonidos/205517__everheat__axe_barrel1.uasset
Version/formato original: 205517__everheat__axe_barrel1.wav 
by [EverHeat] is licensed under CC BY 3.0 (https://creativecommons.org/licenses/by/3.0/)

Project/Content/ModelosPropios/sonidos/79540__kyster__bell-02.uasset
Version/formato original: 79540__kyster__bell-02.wav
by [Kyster] is licensed under CC BY 4.0 (https://creativecommons.org/licenses/by/4.0/)

Project/Content/ModelosPropios/sonidos/97980__oldedgar__winner-bell-game-show.uasset
Version/formato original: 97980__oldedgar__winner-bell-game-show.wav
by [oldedgar] is licensed under CC BY 1.0 (https://creativecommons.org/publicdomain/zero/1.0/)

Project/Content/ModelosPropios/sonidos/709989__audiocoffee__funny-country-loop-ver.uasset
Version/formato original: 709989__audiocoffee__funny-country-loop-ver.wav
by [AudioCoffee] is licensed under CC BY-NC 4.0 (https://creativecommons.org/licenses/by-nc/4.0/)

### 🖼️ Texturas e imágenes utilizadas
Todas las imágenes utilizadas en este proyecto fueron generadas mediante IA de Sora (ChatGPT):
Project/Content/ModelosPropios/controles.uasset
Project/Content/ModelosPropios/forajido.uasset
Project/Content/ModelosPropios/indicadorOro.uasset
Project/Content/ModelosPropios/tiro.uasset
Project/Content/ModelosPropios/puntuacion_ncl1_1.uasset


## 🎤 Entrevista y proceso de desarrollo 
### 🛠️  Descripción del proceso de creación 
Comencé usando el proyecto base proporcionado. Modifiqué la configuración inicial e hice varios ajustes adicionales.
Creé mi mapa, mi nivel y mi pawn. Luego empecé a trabajar en la interacción para agarrar objetos, utilizando tags para identificar diferentes elementos agarrables. También diseñé unas manos que representan los motion controllers. Mediante el uso de Begin Overlap, End Overlap y colisiones, logré implementar la mecánica de agarre con ambas manos.

Después añadí la posibilidad de lanzar los objetos o dispararlos, dependiendo de si se trataba de un hacha o una pistola. Implementé un actor de puntuación que suma puntos al detectar colisiones con ciertos actores, y creé un sistema de ranking que almacena las 5 puntuaciones más altas en un vector.

También incorporé un flujo de juego para que se pueda rejugar la experiencia. Para esto, añadí un "botón" en forma de campana que, al pulsarlo, genera nuevas armas: 2 pistolas, 3 hachas, 2 botellas y 3 armas aleatorias entre estas opciones.

Desarrollé varios objetos que otorgan puntos:

Un muñeco de madera.

Una rata que se mueve aleatoriamente por el espacio.

Un pato que se desplaza horizontalmente y reaparece cada 15 segundos.

Un lingote de oro que otorga 100 puntos.

Por último, cambié el sistema de movimiento. Inicialmente usaba los joysticks, pero ese método generaba mareos y no funcionaba bien, así que implementé movimiento por teletransporte.

### 🧱 Dificultades encontradas 
Una de las principales dificultades fue lograr que el proyecto compilara correctamente en las gafas. Tuve problemas con la configuración del proyecto y con el plugin de MetaXR, ya que en mi portátil Unreal Engine se cerraba al intentar usarlo. Finalmente, tuve que descargar todo en mi PC de sobremesa para poder continuar.

También encontré dificultades al implementar la mecánica de agarre de objetos, ya que a veces parecía que los objetos seguían agarrados incluso después de haber sido lanzados. Afortunadamente, ese problema se resolvió.

En cuanto al teletransporte, tuve un problema porque se ejecutaba en cada frame mientras la tecla estaba pulsada, lo que causaba un comportamiento inesperado. Lo solucioné rápidamente ajustando la configuración del input mapping.

### Siguientes pasos 
Mi idea es añadir más objetos lanzables con diferentes mecánicas, así como más niveles o salas que contengan distintos tipos de objetos que otorguen puntos, como por ejemplo un sombrero que caiga del cielo o un vaso.

También quiero implementar una opción para pausar el juego o reiniciar toda la experiencia desde el principio.

## 📦 Builds
### 📂 Enlaces a los packages (Windows + Android)
Enlace a la carpeta donde tengo la apk de android para las metaquest 3, 
la apk esta dentro de la carpeta Andorid_ASTC y es el archivo **VRRaulleonvalero2-Android-Shipping-arm64.apk**
https://drive.google.com/drive/folders/1-7WAXm9sBPl9ESp56xuHj0kMRs0pMTki?usp=sharing


La version de windows se encuentra en este repositorio, en la carpeta package.

