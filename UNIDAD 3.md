Nombre: Derek Oswaldo Nieto Benitez

Campo 1
Dato de ejemplo: 10101010 10101010 10101010 10101010 10101010 10101010 10101010 10101011 (8 bytes)
Nombre del campo: preambulo
Para qué sirve: permite que los dispositivos receptores sincronicen sus relojes internos con la señal del emisor antes de que lleguen los datos importantes

Campo 2
Dato de ejemplo: FFFF.FFFF.FFFF (6 bytes)
Nombre del campo: direccion MAC de destino
Para qué sirve: indica hacia que dispositivo va dirigido en la red local

Campo 3
Dato de ejemplo: 0001.4321.ABCD (6 bytes)
Nombre del campo: direccion MAC de origen
Para qué sirve: identifica al dispositivo emisor que esta transmitiendo la trama

Campo 4
Dato de ejemplo: 0x0806 (2 bytes)
Nombre del campo: ethertype
Para qué sirve: indica que protocolo de la capa superior esta enca´sulado dentro de la carga util de la trama ethernet

Campo 5
Dato de ejemplo: ¿Quién tiene la IP 192.168.1.2? Responde a 192.168.1.1 (entre 46 y 1500 bytes)
Nombre del campo: carga util
Para qué sirve: Este campo de tamaño variable transporta la información real que se desea transmitir entre los equipos de la red

Campo 6
Dato de ejemplo: 0x3A7F91C2 (4 bytes)
Nombre del campo: Secuencia de Verificación de Trama
Para qué sirve: se utiliza para detectar errores de transmisión en la red. El dispositivo emisor calcula un código numérico basado en los datos de la trama y lo coloca en este campo; al recibir la información, el equipo receptor realiza el mismo cálculo matemático y compara su resultado con el valor recibido para comprobar si la trama llegó intacta o si sufrió alguna alteración en el camino

Switch de Capa 2
Decide por donde reenviar usando solo la direccion  MAC de la trama y su tabla de direcciones MAC; trabaja dentro de una sola red( o una VLAN)

Switch de capa 3
Ademas de conmutar por MAC; puede enrutar usando la direccion IP del paquete y su tabla de rutas, y conecta varias redes o VLAN entre si.

Capa 2 frente a capa 3
Capa 2; lee la MAC, trabaja en una sola red, necesita un router para comunicar redes distintas

Ejemplo de una red a otra
Un equipo de la red 192.168.1.0/24 quiere hablar con la 192.168.2.0

¿Reemplaza un router?
no del todo: el router sigue siendo mejor para conectar con el exterior(WAN, internet)
y para funciones como NAT . El switch de capa 3 se usa en campus y centros de datos para enrutar entre VLAN a alta velocidad

Fibra Optica
La luz viaja por el nucleo y rebota en sus paredes por reflexion total interna, porque el revestimiento que lo rodea desvia la luz de vuelta hacia adentro.

Partes del cable de fibra
De adentro hacia afuera: el nucelo, que conduce la luz; el revestimiento, que la mantiene dentro; el recubrimiento, que protege el vidrio; y la cubierta exterior

Fibra monomodo
Tiene un nucleo muy delgado por donde viaja un solo haz de luz, generado con laser; alcanza decenas de kilometros

Monomodo frente a multimodo
monomodo: nucleo delgado, laser, larga distancia y mayor costo
multimodo: nucleo grueso, led, corta distancia y menor costo 

Componentes de un enlace de fibra
Se necesita el cable de fibra con conectores en sus extremos y un transceptor que convierte la señal electrica en luz; un convertidor de medios

Transceptores
 es un modulo intercambiable que se inserta en el puerto del switch o router y convierte la señal electrica en luz y la luz en señal electrica; se elige el tipo de fibra, la distancia y la velocidad

Tipos de transceptores
Por velocidad: DFP 1gbps, SFP+ 10 Gbps, SFP28 25 Gbps, QSFP +40 gbps y QSFP28 100 gbps

por fibra: SX para multimodo y LX para monomdo

Ventajas de la fibra optica
Ofrece mucho ancho de banda, llega a mayores distancias, es inmune a la interferencia electromagnetica y es mas dificil de intervenir sin ser detectado

Desventajas de la fibra optica
Los equipos y conectores cuestan mas, la instalacion y los empalpes requieren herramientas especializadas , y el cable es fragil si se dobla demasiado.

Donde se usa la fibra optica
En el backbone de internet, en los cables submarinos, en los enlaces entre edificios de un campus y en los centros de datos

UTP frente a fibra optica
UTP: señal electrica, hasta 100m, economico, sensible a la interferencia
Fibra: pulsos de luz, desde cientos de metros hasta decenas de kilometros, mas costosa, inmune a la interferencia

