
<img src="https://github.com/eduroboticfll/MERCURIO-VANGUARD-FE/assets/82280656/cac4b78b-866f-4174-86fb-b2a1a6bfaf08" width="400">


Equipo : VANGUARD

Pais : España 

Nombre 1 : Alvaro Marcos Cascallana

Nombre 2 : Liam Alberdi Camarasa

Nombre 3 : Jagoba Lejarza Zarandona

Entrenador : Sergio Martin Urkijo



## Engineering materials
====
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


## Introducción

Somos un equipo de EDUROBOTIC formado por tres integrantes del colegio Santa Maria, Alvaro, Liam y Jagoba. Hemos querido apuntarnos a esta modalida ya que nos fascino desde el primer momento la idea de programar un coche que condujese solo, esta fue la principal motivacion para apuntarnos. 

## Desarrollo

### Gestión del movimiento.

Para el movimiento del motor, el diseño original del coche utilizaba un motor brushless, similar a los usados en drones. Hemos tenido que cambiar ese motor por un convencional de corriente contínua ya que no hemos sido capaces de hacerlo funcionar debido a que es necesario conectar un variador o ESC a la raspberry y no existe mucha información.

El motor finalmente elegido es un motor "común" típico de montajes robóticos. Hemos adaptado la parte del chasis para su colocación. El motor es controlado por un micro L293D ya que no es recomendable conectarlo directamente a la raspberry. Lo alimentamos desde una Lipo de 11 V y mediante un  regulador de voltaje que cambia los 11 V por 7 V con los que alimentamos el motor.

El motor va unido a un engranaje el cual hace mover a otro engranaje que está unido al eje trasero del coche.
### Gestión de alimentación y sensores

### Gestión de obstáculos
