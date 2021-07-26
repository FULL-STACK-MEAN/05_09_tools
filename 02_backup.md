# Herramientas de backup

## ¿Dónde conseguir las herramientas?

Disponibles en https://www.mongodb.com/try/download/database-tools

Es recomendables ubicar en la misma carpeta de los binarios de mongod, mongos, mongo, etc... para
así aprovechar la ruta en las variables de entorno

C:\Program Files\MongoDB\Server\4.4\bin

## mongodump

Realiza backup a nivel de base de datos o colección

Desde cualquier terminal

mongodump

--host <dirección servidor> | --uri <uri> (si no se indica el valor por defecto es localhost)

--port <puerto servidor>

--db=<base-de-datos>

--collection=<colección>

--out=<ruta>

Prueba

mongodump --port 27017 --db=clinica --out="backup/bck260721

## mongorestore

Restaura un backup a nivel de base de datos o coleccion

mongorestore --port 27017 backup/bck260721

