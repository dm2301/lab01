# lab01
desplegar dos webs, mostrar web 01 y web 02 como contenido,
 los puertos deben estar configurados en 4000 y 4001
gestionar carpetas para orden
hacer uso de gitflow/conventional commits

# Despliegue de Web 01 y Web 02 con Docker

Este proyecto despliega dos aplicaciones web estáticas usando Docker y Nginx.  

## Estructura de carpetas

src/web01/Dockerfile
src/web01/index.html

src/web02/Dockerfile
src/web02/index.html


## Construcción de imágenes

Desde la raíz del proyecto se ejecuto:

docker build -t web01:1.0 src/web01
docker build -t web02:1.0 src/web02

## Para levantar los contenedores 

Primero limpiamos cualquier otro contenedor previo 
Luego se levanta o corre los contenedores en los puertos que se proporcionaron 

Para web01 se uso el puerto 4000
Para web02 se uso el puerto 4001

En mi caso no pude acceder a la web mediante GitHub Codespaces con localhost en lugar de eso se me proporcionaron otros enlaces luego de especificar y agregar los puertos 
 - Para Web01 se uso el puerto https://musical-funicular-x5q7qwvww59qhv9rr-4000.app.github.dev/
 - Para Web02 se uso el puerto https://musical-funicular-x5q7qwvww59qhv9rr-4001.app.github.dev/

En el entorno local si funciona los puertos localhost:4000 y localhost:4001