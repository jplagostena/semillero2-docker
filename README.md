#Semillero 2 - Proyecto Nahual

###Instalación DEV

* Hacer un directorio en el $HOME de tu sistema llamado "nahual" (sin comillas, claro)
* Asegurarse de que este directorio tenga permisos copados de escritura
* Por problemas con el path y docker-compose, creamos un link simbólico del archivo en el directorio padre
  
  
    ln -s ~/nahual/semillero/semillero2-docker/docker-compose.yml ~/nahual/semillero/
    
* Levantar el entorno con `docker-compose up -d`
    
###Documentación API
    
TODO



=======
# semillero2-docker
docker-compose de la nueva versión de Semillero 
