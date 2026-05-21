# Contenedores de Sistemas Gestores de Bases de Datos 


## Comandos Docker con Descripcion 
![ImagenDocker](img/image.png)

| Comando| Descripcion |
| :--- | :--- |
| **docker --version ** |
| ** docker pull nombre_imagen** |
| (https://hub.docker.com/) | 
| ** docker images** | _Visualiza las imagenes |
| ** docker run ** | _Crea un contenedor_ |
| ** docker ps** | _Visualiza todos los contenedores en ejecucion_ |
| ** docker container ls ** | _Visualiza todos los contenedores en ejecucion_ |
| ** docker ps -a** | _Visualiza todos los contenedores en ejecucion y no en ejecucion_ |
| ** docker stop nombre_contenedor o ID** | _Detiene el contenedor |
| ** docker start nombre_contenedor o ID** | _Inicia el contenedor |
| ** docker rm nombre_contenedor o ID** | _Elimina un contenedor que no esta en ejecucion  |
| ** docker rm -f nombre_contenedor o ID** | _Elimina un contenedor que esta en ejecucion  |
| ** docker volume ls** | _Lista de volumenes que tiene docker |
| ** docker volume create nombre_volumen** | _Crea un volumen |
| ** docker volume rs nombre_volumen** | _Elimina el voluemn |
|Fila 1, Celda 2 |
Fila 2, Celda 2 |

## Comandos de contenedores SGBD

```
docker pull docker/getting-started 
```

### Contenedor de tutorial de docker

```
docker run -d --name tutorial-docker -p 80:80 docker/getting-started:latest
```



### Cntenedor de MariaDB

```
docker run -d --name server-MariaDBG3 -p 3342:3306 -e MARIADB_ROOT_PASSWORD=12345  de11b
```

### Contenedor de MariaDB con volumen


### Contenedor de MariaDB sin volumen 



```
docker run -d --name server-MariaDBG3 -p 3342:3306 -e MARIADB_ROOT_PASSWORD=12345  de11b
```


### Contenedor de Postgres con volumen 
```
docker run -d --name server-postgresg3 \
-e POSTGRES_PASSWORD=123456 \
-p 5456:5432 -v vol-postgresg3:/var/lib/postgresql/data \
7e32e
```