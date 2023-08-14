#1 --top-ports 500 (lista los 500 puertos mas comunes)
#2 -p- (listado de todos los puertos tcp/udp)
#3 --open (te lista solo puertos abiertos)
#4 -v (modo verbose)
#5 -n (deshabilitas la resolución DNS)
#6 -TX (0-Paranoico 1-sigiloso (evadir IDS) 2-amable 3-Normal 4-Agresivo 5-Loco) A mayor nº más rápido será pero también menos fiable
#7 -pXX (analizas el nº de puerto especificado)
#8 -Pn (antes de realizar el mapeo comprueba que el host está activo TCP)
#9 -sS (envía un SYN y espera respuesta -si se recibe el SYN/ACK es puerto abierto, si es RST no hay nada)
#10 -sT (igual que #9 pero el SYN lo envía el host, no nmap y es mas lento (este es mejor))
#11 -sU )igual que -Pn pero en UDP
#12 -sn XX.XXX.XXX.XXX/XX (barrido de ping para saber que hosts están activos )



-nmap -p- (listado de todos los puertos tcp/udp) XXX.XXX.XXX.XXX (Ip de la que quieres comprobar)

-nmap --top-ports 500 (lista los 500 puertos mas comunes) XXX.XXX.XXX.XXX (Ip de la que quieres comprobar)

