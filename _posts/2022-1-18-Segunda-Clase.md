---
layout: post
title: SEGUNDA CLASE
---
## Continuación de Vagrant y generalidades
Se inicia la clase mencionando a la comunidad de Facebook y página WEB *nixCraft* que ofrece información sobre Linux entre otras herramientas informáticas de interés para el curso.
Seguido de esto, se hace un recorderis de los comandos vistos en la primera clase de Linux con un resumen de la utilidad de Vagrant.

## Archivos y editores de texto
Previamente vimos el tema de creación de carpetas con el comando en cmd *mkdir **_Nombre_de_carpeta***, en esta es posible generar archivos de texto con *echo **Texto** > **Nombre_del_archivo.txt***, la información contenida en el archivo se puede ver con el comando *cat **Nombre_del_archivo.txt***, el comando *mv* permite mover y/o renombrar archivos a otra ruta, el comando *cp* permite crear una copia del mismo. Ahora trabajaremos en la edición de texto.
### VIM
Editor de archivos de texto por defecto para Linux, para acceder a un archivo mediante VIM solo hay que ejecutar la línea *vim **Nombre_del_archivo.txt*** lo que nos dará acceso al archivo, visualizar (por defecto) y editar el texto que contiene (pulsando la letra 'i'); en el modo de edición podemos agregar y quitar texto según se requiera como se haría en un software de notas normalmente, para salir debemos pulsar la tecla 'escape'. ✍️ :w enter para grabar :q salir se pueden mezclar ! al final para forzar el comando usado entre muchos otros comandos que se pueden consultar en línea.
### Nano (anteriormente Pico)
Es otro editor de texto relativamente más fácil de trabajar que además ofrece una ayuda de los comandos que se pueden usar típicamente una tecla precedida de la tecla 'control'

## Usuarios en LINUX
Es posible crear usuario y modificar sus permisos así como acceder a estos, para ello haremos distintos usos del comando *sudo*, este usuario pertenecerá a un grupo y según estas clasificaciones poseerá unos permisos especiales para la manipulación de los archivos, asimismo existirán permisos por default para otros usuarios externos al grupo (como invitados), estas acciones serán escribir (**w**rite), leer (**r**ead) y ejecutar (e**x**ecute) que pueden ser modificadas por root o el *dueño o chown* del archivo. Con el cmando *chmod* se pueden otorgar y retirar estos permisos
### Permisos
* rwx -> n
* 111 -> 7: rwx
* 110 -> 6: rw-
* 101 -> 5: r-x
* 100 -> 4: r--
* 011 -> 3: -wx
* 010 -> 2: -w-
* 001 -> 1: --x
* 000 -> 0: ---
Ejemplo: *chmod 764 **Nombre_del_archivo.txt*** daría permisos de leer, escribir y ejecutar para el usuario, leer y escribir para el grupo, pero solo leer para otros.

## Sabores de Linux
Para concluir con la unidad de Linux, se hizo un repaso de las diferentes distribuciones (distros) o sabores de Linux conociendo sus padres, derivados, historia y aplicaciones, repasando algunas diferencias en sus arquitecturas y comandos.
### sudo apt (update-get-install-search) para actualización, instalación y búsqueda de programas
Se acaba la clase con la instalación de MariaDB, un repaso de los puertos y el modelo OSI.
