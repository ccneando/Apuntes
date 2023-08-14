#1 --top-ports 500 (lista los 500 puertos mas comunes)

#2 -p- (listado de todos los puertos tcp/udp)

#3 --open (te lista solo puertos abiertos)

#4 -v (modo verbose - información descriptiva en tiempo real)

#5 -n (deshabilitas la resolución DNS -algo recomendado - tardas menos y levantas menos sospechas)

#6 -TX (0-Paranoico 1-sigiloso (evadir IDS) 2-amable 3-Normal 4-Agresivo 5-Loco) A mayor nº más rápido será pero también menos fiable y mas posible que te detecten

#7 -pXX (analizas el nº de puerto especificado)

#8 -Pn (considera que el host o puerto está activo )

#9 -sS (envía un SYN y espera respuesta -si se recibe el SYN/ACK es puerto abierto, si es RST no hay nada)

#10 -sT (igual que #9 pero el SYN lo envía el host, no nmap y es mas lento (este es mejor))

#11 -sU )igual que -Pn pero en UDP

#12 -sn XX.XXX.XXX.XXX/XX (barrido de ping para saber que hosts están activos )

#13 -sV (detectar servicio y versión de los puertos que tiene que analizar)

========== EVASIÓN DE FW e IDS==============

#14 -f (ALTAMENTE RECOMENDADO -sirve para fragmentar los paquetes y así evadir los firewall y tener información de puertos en estado "Filtrado")

#15 --mtu (nunca combinar con #14)(es igual que #14 pero aquí puedes especificar el tamaño de fragmento a enviar, siempre que sean múltiplos de 8)

#16 (xxx.xxx.xxx.xxx IP de destino) -D (xxx.xxx.xxx.xxx ip de señuelo)
(Esto se hace por que hay reglas en el firewall que solo permiten que cierta IP pueda ver si un puerto está abierto -  sería falsificar la IP de origen¡)

#17 --source-port XX (especificas el puerto por el que quieres que se envíen los datos, en vez de uno aleatorio.)

#18 --data-length XX (58+XX)algunos firewall reconocen el tamaño de los datos y lo bloquean, con esto lo que haremos será agregar mayor tamaño para evitar esa detección/bloqueo)

#19 --spoof-mac XXXXXXXX (hay equipos que solo aceptan datos cuando vienen de una MAC en concreto, con esto lo que haríamos sería falsificarla)

#20 -sS (no se llega a completar la conexión y por lo tanto no queda registro ni alertas en muchos firewall / SYN - SYN-ACK/RST)

#21 --min-rate XXXX (Esta técnica permite al usuario controlar la velocidad de los paquetes enviados para evitar la detección del Firewall. 5000 está bien.)

#22 -sC  (análisis actual del conjunto por defecto de scripts (algunos pueden ser intrusivos).

#23 --script "XXXXX" (con esto lanzamos los scripts basados en su categoría)

#24 --script XXXX (ejecutas un script en concreto)

#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14
#14




-nmap -p- (listado de todos los puertos tcp/udp) XXX.XXX.XXX.XXX (Ip de la que quieres comprobar)

-nmap --top-ports 500 (lista los 500 puertos mas comunes) XXX.XXX.XXX.XXX (Ip de la que quieres comprobar)

