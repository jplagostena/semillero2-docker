# Semillero 2 - Proyecto Nahual

### Requisitos

El sistema corre con Docker y docker-compose para orquestar containers al menos en desarrollo.

### Instalación DEV

* Hacer un directorio en el $HOME de tu sistema llamado "nahual/semillero" (sin comillas, claro)

    `mkdir nahual/semillero`
* Asegurarse de que este directorio tenga permisos de escritura
* En este directorio hacer el checkout de los 3 proyectos de Semillero 2


    `git clone git@github.com:nahual/semillero2-web.git
    
    git clone git@github.com:nahual/semillero2-docker.git
    
    git clone git@github.com:nahual/semillero2-api.git`
    
* Por problemas con el path y docker-compose, creamos un link simbólico del archivo en el directorio padre

  
    ln -s ~/nahual/semillero/semillero2-docker/docker-compose.yml ~/nahual/semillero/

La idea es que nos quede un link simbólico al docker-compose.yml con las 3 carpetas de los proyectos.
    
* Levantar el entorno con `docker-compose up -d`

* El docker-compose.yml levanta 3 contenedores:
    * semillero2-web es una imágen que hereda de node-9 y usa angular y el server embebido de angular.
    * semillero2-api hereda de maven y usa java 8.
    * una base de datos MariaDB con la hermosura de root/{nada} como password (si, lo se, estamos para la ekoparty (?))
        *PUERTO: el puerto es el __3307__ para evitar el clashing con instalaciones ya existentes de MariaDB | MySQL  
    

#### Instalación API DEV

[Ver esto!](https://github.com/nahual/semillero2-api)

### Documentación API
    
La documentación de la API está escrita en RAML 0.8. 

El HTML generado se puede ver en el siguiente [link](https://rawgit.com/nahual/semillero2-api/development/apiV2.html)





