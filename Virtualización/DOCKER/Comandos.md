-Crear un documento "Dockerfile" que define la configuración de las imágenes
FROM XXX (nombre de la imagen) 

MAINTAINER XXXXXX (quien está detrás de todo esto)

RUN XXXXXXX (comandos de instalación de software)
ENV DEBIAN_FRONTEND noninteractive (deshabilitas el modo interactivo)
EXPOSE xx (numero de puerto que quieres exponer)
ENTRYPOINT XXXXX(comandos que ejecutará nada mas arrancar el docker)





-Construir una imagen de Docker desde un "DockerFile"
docker build -t XXX (descargará la imagen con esa etiqueta) XXXX (ruta del Docker File)

doker images (listas todas las imágenes)
docker pull xxxx (nombre de la imagen a descargar)

-Cuando se haga cualquier cambio en el Dockerfile hay que:
docker build -t XXX (nombre de la imagen) XXXX (ruta del Docker File) 

-Como crear un contenedor de docker 
docker run -dit (segundo plano / interactivo /terminal)  --name XXX (nombre del container) XXXXX (nombre de la imagen que creaste previamente en la que se va a vbsar este container)

-Ver contenedores corriendo / Activos
docker ps

-acceder al contenedor 
docker exec -it (interavo / terminal ) XXXXX (nombre del container creado) bash (comando: y se ejecuta en el container, y como tenemos el comando -t se nos cambia la terminal )

-Parar un container
docker stop XXXXXX (id del container)

-Borrar un container que no esté activo /no se borra la imagen
docker rm XXXXX (id del container)

-Borrar un container que SI esté activo /no se borra la imagen
docker rm XXXXX (id del container) --force

-Borrar una imagen
docker rmi XXXX (id de la imagen )

-borrar todas las imagenes
docker images -q (muestra los id de las imagenes)
docker rmi $(docker images -q)

-p XX:XX  (le indicas que el puerto de la máquina es la de origen del container  )

-v XXXXXX:XXXXXX (ruta que quieres tener montada en la ruta de dentro del container)