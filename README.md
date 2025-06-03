# 🎯 Simulador de Tiro al Blanco en Realidad Virtual (Unreal Engine)

## 📄 Documentación
### 🕹️ Descripción de la experiencia
Juego de realidad virtual desarrollado en Unreal Engine para la Universidad de Alicante, 
donde encarnas a un vaquero y debes demostrar tu puntería usando hachas y revólveres para acertar en objetivos. 
Una experiencia inmersiva que combina acción y precisión en un entorno del Viejo Oeste.

## 🎮 ¿Cómo jugar?
Empezaras en una sala con un mensaje explicativo que se resume en avanzar a la zona de disparo,
Cuando estes en esa zona deberas tocar una campana(situada a la izquierda y de color amarillo)
con la p en ordenador y con la B en las metaquest.
Despues apareceran objetos cerca de la campana que podras coger y utilizar para lanzar a los muñecos,
ratas, patos y lingote de oro que estan situados en la zona de disparo, cuando te quedes sin objetos,
vuelve a pulsar la campana para subir la puntuacion al ranking y generar nuevos objetos y una nueva ronda.
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

![CONTROLESteclado](https://github.com/user-attachments/assets/ea0a8347-b8e1-4881-a55d-ee0ac18f6349)


**Metaquest**

B ➡ Para tocar la campana al colisionar la mano con ella

joystick derecho ➡ rotar

joystick izquierdo ➡ Moverse

Gatillo izquierdo ➡ Coger objeto con la izquierda

Gatillo derecho ➡ Coger objeto con la derecha

X ➡ Lanzar objeto con la izquierda

A ➡ Lanzar objeto con la derecha

![controles](https://github.com/user-attachments/assets/0914d9d8-d5c1-49d3-b7b8-2aead8ed5a95)

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
Empeze usando el proyecto base proporcionado, cambie la configuración e hice mas ajustes.
Cree mi mapa,mi nivel  y mi pawn, despues empece con la interaccion de agarrar objetos, donde use 
las tags para crear varios objetos agarrables ademas de unas manos que representan los motion controllers
y comprobando los begin y end overlaps y usando collisiones hice la iteracion de agarrar objetos con ambas manos.
Despues hice que se pudieran lanzar los objetos o disparar dependiendo de si el objeto era hacha o pistola,
hice un actor puntuacion que sumaba puntos cuando los actores colisionables recibian un golpe y un ranking 
que usa un vector con las 5 maximas puntuaciones obtenidas.
Luego implemente un flujo de juego para poder rejugar la experiencia, por lo que use
un "boton" representado por una campana que al pulsarla genera las armas 2 pistolas, 3 hachas, 
2 botellas y tres armas aleatorias entre estas 3 posibles.
Hice varios objetos que dan puntos, el primero un muñeco de madera, luego una rata que se mueve por el espacio
de forma aleatoria, tambien hice un pato que se desplaza horizontalmente y respaunea cada 15 segundos 
y por ultimo hice un lingote de oro que da 100 puntos.
### 🧱 Dificultades encontradas 
Que compile en las gafas, he tenido problemas con la configuracion del proyecto ademas del plugin de metaXR 
ya que en mi portatil crasheaba al meterlo en unreal y tuve que descargar todo en mi PC de sobremesa.
Tuve dificultades en la implementacion del agarre de objetos ya que aveces se quedaban como que todavia los tenia
agarrados cuando ya habian sido lanzados, pero ese problema fue resuelto.

### Siguientes pasos 
Intentar meter mas objetos lanzables con diferentes mecanicas ademas de mas niveles o salas con diferentes
objetos que puntuen, por ejemplo un sobrero que caiga del cielo o un vaso.
Tambien meter una opcion de pausa o de reiniciar todo desde el principio.

## 📦 Builds
### 📂 Enlaces a los packages (Windows + Android)
Enlace a la carpeta donde tengo la apk de android para las metaquest 3, 
la apk esta dentro de la carpeta Andorid_ASTC y es el archivo **VRRaulleonvalero-Android-Shipping-arm64.apk**
https://drive.google.com/drive/folders/1fnmnsdRfU8qhcwb7NNCSpk1Fe7wU-jcH?usp=sharing


La version de windows se encuentra en este repositorio, en la carpeta package.

