
<img src="https://github.com/eduroboticfll/MERCURIO-VANGUARD-FE/assets/82280656/cac4b78b-866f-4174-86fb-b2a1a6bfaf08" width="400">


Equipo : VANGUARD

Pais : España 

Nombre 1 : Alvaro Marcos Cascallana

Nombre 2 : Liam Alberdi Camarasa

Nombre 3 : Jagoba Lejarza Zarandona

Entrenadores : Sergio Martin y Nuncy Nikita 



## Engineering materials

- Coche Impreso en 3D
- Tornillos adaptados al coche
- Raspberry Pi 3
- Camara Raspberry 
- Motor brushless y ESC 
- 1 Bateria LiPo 3S
- Micro L293D para controlar motor. 
- Servo motor para la dirección.
- Motor DC.
- Gomas para la suspension 
- 3 sensores HC-SR04 
- Pulsador 
- Power bank 


## Introducción

Somos un equipo de EDUROBOTIC formado por tres integrantes del colegio Santa Maria, Alvaro, Liam y Jagoba. Hemos querido apuntarnos a esta modalidad, ya que nos fascinó desde el primer momento la idea de programar un coche que condujese solo, esta fue la principal motivación para apuntarnos. Nunca hemos hecho algo parecido a esto, lo más cerca de haber hecho algo así ha sido en la First Lego League, creando un coche para resolver pruebas (Coger, Mover, Colgar, Tirar...) Para nosotros haber creado este coche es un honor. Siempre  recordaremos ese día " El día que creamos a  

## Chasis 

Nuestro innovador vehículo dispone de un sistema de suspensión McPherson en el tren delantero, el cual hace referencia a nuestro elevado nivel de entendimiento en la materia. No conforme con ello, también hemos acoplado otra suspensión de eje rígido en el tren trasero. Lo hemos probado por intrépidos y rugosos caminos, los cuales ha superado sin ningún inconveniente. Nuestro sistema de dirección accionado por un servomotor se adapta a la altura que tiene en cualquier momento la suspensión. Sin duda una gran proeza por parte del equipo Vanguard.
## Desarrollo

### Gestión del movimiento.

Para el movimiento del motor, el diseño original del coche utilizaba un motor brushless, similar a los usados en drones. Hemos tenido que cambiar ese motor por un convencional de corriente contínua, ya que no hemos sido capaces de hacerlo funcionar debido a que es necesario conectar un variador o ESC a la raspberry y no existe mucha información.

El motor finalmente elegido es un motor "común" típico de montajes robóticos. Hemos adaptado la parte del chasis para su colocación. El motor es controlado por un micro L293D, ya que no es recomendable conectarlo directamente a la raspberry. Lo alimentamos desde una Lipo de 11 V y mediante un  regulador de voltaje que cambia los 11 V por 7 V con los que alimentamos el motor.

El motor va unido a un engranaje, el cual hace mover a otro engranaje que está unido al eje trasero del coche.
### Gestión de alimentación y sensores
Hemos utilizado 3 sensores  HC-SR04, con ellos medimos las distancias de las paredes frontales, laterales. También hemos instalado una cámara frontal raspberry pi cam con la cual, esta cámara saca una foto cada 0,1 segundos, al sacar la foto lo que hace es ver donde están los píxeles de cada color. Un ejemplo: la cámara cuando ve un cuadrado de píxeles verdes, lo que hace es girar hacia la izquierda, y si la cámara detecta un cuadrado de píxeles rojos, gira hacia la derecha.
### Gestión de obstáculos
Hemos intentado mediante una pi CAM detectar los obstáculos, usando Open CV. El procedimiento sería el siguiente, La cámara hace una foto, con esa foto lo que detecta son los píxeles verdes u rojos. Al detectar los píxeles verdes u rojos, lo que tiene que hacer es girar 
hacia la izquierda o derecha dependiendo el color de cada pixel. 
![image](https://github.com/eduroboticfll/MERCURIO-VANGUARD-FE/assets/82280656/0e49348a-5c6f-4f1b-bf51-db23faa1c6eb)
