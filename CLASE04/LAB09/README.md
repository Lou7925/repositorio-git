
# CLASE 04 - LAB09

Despliega un proyecto Drupal utilizando Docker


## 01 - Clonar el repositorio del proyecto en nuestro equipo

```bash
$ git clone https://github.com/wodby/docker4drupal.git
```
![Clone](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/git_clone.png)

## 02 - Ejecutar docker-compose para levantar todo el sistema

```bash
$ cd docker4drupal
$ docker4drupal$ docker-compose up -d
```
![docker-compose](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_compose.png)

Se verifica que todos los contenedores estén UP con el siguiente comando:
```bash
docker ps
```
![docker-ps](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_ps.png)

Luego de realizar pruebas, se detienen los contenedores con:

```bash
docker stop
```
![docker-stop](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_stop.png)
![docker-stop-ok](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_stop_ok.png)

Luego se borran los contenedores ejecutando:

```bash
docker rm
```
![docker-rm](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_rm.png)
![docker-rm-ok](https://github.com/dfernandezlecler/diegofl-web/blob/master/LAB09/docker_rm_ok.png)


## Authors

- [@dfernandezlecler](https://www.github.com/dfernandezlecler)
- [@Lou7925](https://www.github.com/Lou7925)
- [@edwinler](https://www.github.com/dfernandezlecler)
- [@cecilia](https://www.github.com/dfernandezlecler)

