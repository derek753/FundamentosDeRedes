Red y Host
Toda direccion tiene dos partes: la parte de red

### Direcciones publicas
Las direcciones publicas son publicas en todo internet y las asigna un proveedor de servicio.

Un equipo con direccion publica es alcanzable desde internet; lass privadas, no.

### Direcciones privadas
Se usan solo dentro de una red y no se enrutan en internet: 10.0.0.0/8. 172.16.0.0/12 y 192.168.0.0/16. Para salir a internet usan NAT.

### Direcciones especiales 

127.0.0.1 es el loopback (el propio equipo) y 169.254.0.0/16 es la asignacion automatica (APIPA) cuando falla el DHCP
0.0.0.0/0 es la ruta predeterminada

### Direcciones IPv4

Una direccion 

### DHCP
El cliente obtiene su configuracion en cuatro pasos, DORA: discover, offer, request.

### Para que sirve el DHCP
Es un servicio que asigna direcciones IP automaticamente a los equipos de la red.
Evita configurar cada equipo a mano y los conflictos por direcciones duplicadas.

# Los cuatro mensajes de DHCP

| Paso | Mensaje     | Quién lo envía      | Qué hace                            |
| :--: | ----------- | ------------------- | ----------------------------------- |
|  1   | Discover    | Cliente (broadcast) | Busca un servidor DHCP en la red    |
|  2   | Offer       | Servidor            | Ofrece una dirección IP disponible  |
|  3   | Request     | Cliente (broadcast) | Pide la dirección ofrecida          |
|  4   | Acknowledge | Servidor            | Confirma y entrega la configuración |

### Tiempo de consecion
La direccion se entrega en prestamo por un tiempo de concesion, no de forma permanente.
El cliente renueva a la mitad del tiempo; en windows, ipconfig/release liera la direccion e ipconfig/renew.

# El pool de direcciones

### Configuración DHCP

| Campo | Valor |
|---|---|
| Servicios | Encendido |
| Pool Name | DHCP_P1 |
| Gateway por Defecto | 201.10.220.90 |
| Servidor DNS | 201.10.220.90 |
| Inicio de la Dirección IP | 201.10.248.0 |
| Subnet Mask | 255.255.252.0 |

### ¿Cómo funciona?

- El servidor reparte direcciones de un pool (rango) y entrega con ellas:
  - Máscara de subred.
  - Puerta de enlace.
  - DNS.

- Las direcciones fijas de servidores, impresoras y routers se excluyen del pool o se reservan por dirección MAC.


### Puertos y relevo de DHCP
DHCP usa UCP: el servidor escucha en el puerto 67 y el cliente en el 68.
El broadcast no cruza routers: un router con ip helper address reenvia las solicitudes a un servidor de otra red.


### Capas
Capa 2
que es ? Se encarga de la comunicacion entre dispositivos que estan conectados de una misma red 
para que sirve ? Permite transferir datos entre dispositivos de una red local, detecta errores  durante la transmision de datos, Utiliza direcciones MAC para identificar dispositivos, organiza la informacion en tramas.

Capa 3
que es ? Conecta diferentes redes y determina la ruta que debe seguir los datos para llegar a su destino 
para que sirve ? Permite la comunicacion entre diferentes redes, utiliza direcciones IP para identificar dispositivos , determina la mejor ruta para enviar los datos , permite que los routers dirijan la informacion

Capa 4
que es ? Transporta los datos entre los dispositivos de origen y los dispositivos de destino
para que sirve ? Divide los datos en segmentos para enviarlos, controla los datos correctamente, Organiza los datos para que lleguen en orden, controla el flujo de informacion , utiliza protocolos como TCP y UDP