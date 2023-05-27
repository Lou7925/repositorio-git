

Iniciando el Contenedor MongoDB 


Ejecutar un contenedor que corre MongoDB y con el cual nos conectaremos por medio de Python

1. Iniciar el container de MongoDB utilizando el comando docker run -d -p 27017:27017 --name m1 mongo


![Iniciando MongoDB](/repositorio-git/image/Contenedor_MongoDB.PNG)

    i. Puedes conectarte al contenedor de Mongo con docker exec -it m1 /bin/bash y luego conectarte a MongoDB por medio del comando mongosh
    ii. Para salir de la terminal interactiva del contenedor, primero hay que salir de MongoDB tecleando el comando exit, y una vez fuera podemos   tecler la combinación Ctrl+P y Ctrl+Q para salir


![Conectando MongoDB](/repositorio-git/image/Conectando_MongoDB.PNG)

2. Utilizaremos los scripts de Python existentes en la carpeta para la colección de mongo, utilizando la librería https://api.mongodb.com/python/current/tutorial.html

     i. Instalar la librería de mongo por medio del comando pip install pymongo
    ii. Ejecuta los scripts con python populate.py y python find.py
   iii. Revisa los registros por medio del CLI de mongo o de tu DBMS favorito

![Instalando Libreria](/repositorio-git/image/Instalando_Libreria_Mongo.PNG)

![Ejecutando los Script de Python](/repositorio-git/image/Script_Python.PNG)
