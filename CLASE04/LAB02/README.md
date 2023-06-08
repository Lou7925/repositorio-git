
# CLASE 04 - LAB02

## Laboratorio de Docker

## Ejecutamos un contenedor que corre MongoDB, con el cual nos conectaremos por medio de Python


### 01 - Iniciar el container de MongoDB

Creamos el container:

```bash
docker run -d -p 27017:27017 --name m1 mongo
```

Nos conectamos al container:

```bash
docker exec -it m1 /bin/bash
```

Luego nos conectamos a MongoDB con el comando:

```bash
mongosh
```

Para salir de la terminal interactiva del container, primero debe salir de MongoDB con:

```bash
exit
```

    
### 02 - Utilizaremos los scripts de Python existentes en la carpeta para la colección de Mongo, utilizando la librería https://api.mongodb.com/python/current/tutorial.html

Instalamos la librería de Mongo por medio del comando:

```bash
pip install pymongo
```

Ejecutamos los Scripts:

```bash
python populate.py
```
```bash
python find.py
```

Se verifica el funcionamiento revisa los registros por medio del CLI de Mongo

Luego se detienen y se borran los contenedores ejecutando:
```bash
docker stop m1
```
```bash
docker rm m1
```

### Screenshots
#### 01 - Instalar container MongoDB

![docker_run](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB02/docker_run.png)

#### 02 - Ingresar al container de MongoDB

![docker_exec](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB02/docker_exec.png)

#### 03 - Ingresar a MongoDB

![mongodb](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB02/ingresar_container.png)

#### 04 - Eliminar contenedor

![remove](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB02/remove_container.png)











## Authors

- [@dfernandezlecler](https://www.github.com/dfernandezlecler)
- [@Lou7925](https://www.github.com/Lou7925)
- [@edwinler](https://www.github.com/dfernandezlecler)
- [@cecilia](https://www.github.com/dfernandezlecler)

