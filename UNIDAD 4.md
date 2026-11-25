
### IPv4
es el protocolo de la capa de red que direcciona y enruta los paquetes entre las redes, usando direcciones de 32 bits (unos 4.300 millones en total)

### Historia de IPv4
se definio en 1981 dentro de la familia TCP/IP, diseñada por Vint Cerf y bob kahn
En 1983 ARPANET

### Como se agotaron las direcciones
Las 4,300 millones de direcciones parecían suficientes, pero se repartieron en bloques por clases: una Clase A daba más de 16 millones a una sola organización. Además, los dispositivos conectados crecieron sin parar.
En 2011 la IANA entregó sus últimos bloques a los registros regionales. Se alargó la vida de IPV4 con CIDR, las direcciones privadas y NAT; la solución definitiva es IPv6.

### Diferencias entre ip publica y privada

## 1. IP privada

Es una dirección IP que se utiliza dentro de una red local (LAN), por ejemplo, en tu casa, universidad o empresa.

- Identifica dispositivos dentro de una misma red.
    
- No es accesible directamente desde Internet.
    
- Puede repetirse en diferentes redes privadas.
    
- La asigna normalmente el router.
    

Ejemplo: Tu celular, computadora y Smart TV están conectados al mismo Wi-Fi. Cada uno tiene una IP privada diferente.

Ejemplos de IP privada:

- 192.168.1.10
    
- 192.168.1.15
    
- 10.0.0.5
    

## 2. IP pública

Es la dirección IP que identifica tu conexión o red frente a Internet.

- Permite que tu red se comunique con otras redes en Internet.
    
- Es asignada por tu proveedor de Internet (ISP).
    
- Debe ser única globalmente entre las direcciones públicas.
    
- Puede ser dinámica o estática.
    

Ejemplo: Cuando visitas Google, el servidor puede identificar la IP pública desde la que llega tu solicitud.

### Caracteristicas de IPv4
Es sin conexion (cada paquete viaja por separado), de mejor esfuerzo (no garantiza la entrega) e independientemente del medio

### Encabezado IPv4
El encabezado mide 20 hytes como minimo y lleva la ip de origen, la ip de destino, el ttl (limite de saltos) y el campo protocolo (TCP, UDP, o ICMP)

### IPv6
Usa direcciones de 128 bits y se creo porque las direcciones ipv4 se agotaron; permite un numero practicamente ilimitado de dispositivos

### Cuantas direccines tiene IPv6
Con 128 bits hay 2"128 direcciones: unos 340 sextillones. Cada subred estandar por si sola tiene 2" direcciones, mas de 18 trillones 

### Ventajas de IPv6
Ofrece un espacio de direcciones enorme, un encabezado simplificado de 40 bytes, autoconfiguracion de direcciones y no usa broadcast: lo reemplaza el multicvast

### Division de red en grupos 
Una red grande se divide en subredes: grupos de dispositivos organizados por ubicacion, funcion o departamento, vcada uno con su propio rango de direcciones

### Porque dividir una red
Al dividir se reduce el trafico de broadcast, mejora el rendimiento, se aplicn politicas de seguridad por grupo y se facilita la aministracion