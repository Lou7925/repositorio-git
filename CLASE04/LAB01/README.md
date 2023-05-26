
# CLASE 04 - LAB01

Primer laboratorio de Docker


## 01 - Crear Script para instalación automática de NGNIX

Script para la descargar e instalar la imagen de NGINX desde Docker Hub automaticamente en nuestro equipo:

```bash
#!/bin/bash
#Script para la descargar e instalar la imagen de NGINX desde Docker Hub automaticamente

echo "Descargamos la imagen de NGNIX 1.22.1 desde Docker Hub"

docker pull nginx:1.22.1-alpine3.17-slim
```
    
## 02 - Instalar contenedores de MySQL y de PHPMyAdmin y conectarlos entre si

Instalamos e iniciamos el contenedor de MySQL:

```bash
docker run --name=db -p 3306:3306 -e MYSQL_ROOT_PASSWORD=secret-pw -d mysql:8
```
Instalamos e iniciamos el contenedor de PHPMyAdmin:

```bash
docker run --name=my-admin -p 82:80 --link db:db -d phpmyadmin
```

Se verifica su funcionamiento corriendo desde http://localhost:82/, e introduciendo las credenciales para loguearse.
Luego de realizar pruebas, se detienen los contenedores con:
```bash
docker stop
```
Luego se borran los contenedores ejecutando:
```bash
docker rm
```
## Screenshots
### 01 - Crear Script para instalación automática de NGNIX
Script:
![](https://drive.google.com/file/d/1RDfULuMY2h7TI1Fc9wuKZJq8x29O1vV5/view?usp=share_link)

Ejecución del Script:
![](https://drive.google.com/file/d/1-27W9hSl2BQFRdf4KO5SjnsimgqiyxG3/view?usp=share_link)

### 02 - Instalar contenedores de MySQL y de PHPMyAdmin y conectarlos entre si
Instalación de MySQL:
![](https://drive.google.com/file/d/17Vwc7Ldy6vUF40RQ_u_1N9qd5lo_ESLw/view?usp=share_link)

Instalación de PHPMyAdmin:
![](https://drive.google.com/file/d/1FszXc5rmUatclaTUhV1zgZvsNxYa3kmR/view?usp=share_link)

Listado de contenedores:
![](https://drive.google.com/file/d/1J5iMx9S0vUa5YyhlG-qv1jCthIZYRrYr/view?usp=share_link)

Prueba de Funcionamiento de PHPMyAdmin:
![](https://drive.google.com/file/d/1DWIw_URkPjs1I6kWkOwbuESDq8HI_q8d/view?usp=share_link)

Stop de contenedores:
![](https://drive.google.com/file/d/1EbLl45PkDrlbeloj8mQ-k0l3ZRckddWQ/view?usp=share_link)

Borrado de contenedores:
![](https://drive.google.com/file/d/15eY2yla9m45wld4QJQd9Y5MrXPC8aGGA/view?usp=share_link)









## Authors

- [@dfernandezlecler](https://www.github.com/dfernandezlecler)
- [@Lou7925](https://www.github.com/Lou7925)
- [@edwinler](https://www.github.com/dfernandezlecler)
- [@cecilia](https://www.github.com/dfernandezlecler)

