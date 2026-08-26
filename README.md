HW-04 - IPSec Site-to-Site

Descripción

En esta práctica se configuraron dos redes con subredes diferentes, conectadas mediante un router que simula Internet.

Red A: 192.168.10.0/24

Red B: 192.168.20.0/24

R1-SEDE-A (WAN): 10.0.0.1

R2-SEDE-B (WAN): 20.0.0.2

Servidor HTTPS: 192.168.20.10

Topología

La comunicación se realiza desde una computadora ubicada en la Red A hacia un servidor web ubicado en la Red B.

PC-A -- SW-A -- R1-SEDE-A -- R-INTERNET -- R2-SEDE-B -- SW-B -- SERVER-HTTPS

Prueba HTTPS

Desde la computadora de la Red A se realizó una solicitud HTTPS al servidor de la Red B mediante:

https://192.168.20.10

El servidor respondió correctamente mostrando el mensaje:

Servidor Sede B

Conexión HTTPS funcionando correctamente

Evidencia



IPSec

La práctica contempla una VPN IPSec Site-to-Site entre los routers R1-SEDE-A y R2-SEDE-B utilizando tunnel mode, con el objetivo de proteger el tráfico entre las redes:

192.168.10.0/24

192.168.20.0/24

Archivo Packet Tracer

El archivo .pkt correspondiente a la práctica se encuentra incluido en esta rama.

## Topología

![Topología de la red](topologia.png)

## Prueba HTTPS

Desde la Red A se realizó una solicitud al servidor HTTPS ubicado en la Red B.

![Prueba HTTPS](evidencia-https.png)

## Verificación del túnel IPSec

Se verificó el establecimiento de la asociación IPSec y el cifrado de tráfico entre ambas redes.

![Verificación IPSec](evidencia-ipsec.png)