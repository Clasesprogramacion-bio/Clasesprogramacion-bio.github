---
layout: post
title: OCTAVA CLASE
---
## MONGODB
Se inicia la clase con la instalación del software proveedor de servicio documental gratuito y de código abierto MongoDB con el que se gestionará las bases de datos no relacionales que se trabajarán en el curso, para ello se descarga el instalador y se configura sus parámetros como servicio de Windows. Se continúa con la definición de las características de la aplicación,su historia y contexto actual.

### Introducción al shell de MongoDB y comandos básicos:
Se definen los comandos básicos para acceder al servicio y al shell de Mongo que empleará las funciones definidas para este. 
* El comandos básicos *Use {dbs_name}* tiene una función similar al usado en MySQL de crear o trabajar sobre una base de datos.
* El comando *show dbs* lista las bases de datos existentes en la dirección de almacenamiento. 
* El comando *db.dropDatabase()* permite borrar   la base de datos sobre la que estamos ubicados.
* El comando *db.createCollection({name_collection})* crea una colección de datos dentro de la base de datos que estamos usando.
* El comando *show collections* muestra las colecciones existentes dentro de la base de datos.
* El comando *db.{name_collection}.drop()* borra la colección nombrada como name_collection.
* El comando *db.{name_collection}.replace()* reemplaza datos según un filtro.
* * El comando *db.{name_collection}.delete()* borra la información guardada en un documento según el filtro.
Estos comandos pueden tener un One o un Many al final lo que ejecuta la función sobre el primer dato que encuentra o todos, respectivamente.

La creación de datos en MongoDB se da mediante documentos generados sobre notación de JAVASCRIPT en formato **clave:valor**, esta genera por defecto un campo de *_id* concepto similar al de primary key en MySQL, identificación que lo diferencia de otros datos aunque este también puede ser asignado manualmente por medio de un objeto *objectId* de valor hexadecima único.

### Algunos métodos de los documentos en MongoDB:
* **find()**: permite realizar la consulta de documentos por campos específicos de estos.
* **remove()**: permite eliminar documentos según un campo pasado.
* **update()**: actualiza campos o documentos completos, se debe tener la misma precaución que en MySQL para no actualizar todos los registros sino solo los que se especifiquen.

MongoDB permite embeber (object.attribute) hasta en 100 niveles de profundidad y referenciar ($ref: "id", $id: objectId)documentos de otras colecciones, la aplicación de estos operadores mejora tiempos de operación al tiempo que facilita la consulta y disminuye la duplicidad de datos; no obstante, se debe entender que no es lo mismo referenciar que relacionar.

### Ejercicio de base de datos de directorio en MongoDB:
Se desarrolló una base de datos básica que incluye información personal de personas haciendo uso de los métodos y funciones previamente descritos.

### Creación de base de datos tipo JSON en JAVASCRIPT y manejo con MongoDB:
Asimismo, se desarrolló un documento que contuviera datos de una película para comprobar su manejo con MongoDB
