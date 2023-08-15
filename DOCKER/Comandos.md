-Crear un documento "Dockerfile" que define la configuración de las imágenes
FROM XXX (nombre de la imagen) 

MAINTAINER XXXXXX (quien está detrás de todo esto)

RUN XXXXXXX (estos comandos se ejecutarán nada mas crear el container)

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

-Borrar un container
docker rm XXXXX (id del container)