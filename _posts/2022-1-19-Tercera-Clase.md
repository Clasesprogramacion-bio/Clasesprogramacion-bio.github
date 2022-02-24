---
layout: post
title: TERCERA CLASE
---
## Bases de datos relacionales
Consultadas por el servidor WEB para acceder a información contenida en ellas; estas deben contener las relaciones existentes, estas son asociaciones entre las entidades o tablas de datos identificadas por una clave primaria. Las claves primarias son campos únicos que identifican y diferencian una entidad de otra como la cédula a una persona.

### Motores de búsqueda
* MySQL
* MariaDB
* PostgreSQL
* Oracle

### Ejemplo: Base de datos de un almacén
Un almacén puede guardar la información de sus clientes mediante bases de datos relacionales, las entidades que puede esgrimir son el cliente, las ventas y los productos que están relacionados por una factura así como identificados por una clave primaria que son la cédula, el código de barras y número de factura.

### Pasos para crear una base de datos relacional:
1. Determinar los campos o datos de interés
2. Identificar las tablas o entidades
3. Se agrupan los campos según la entidad en tablas apartadas
4. Se define el campo de clave primaria para cada entidad
5. Definición de relaciones que tienen las tablas o entidades entre sí (si existen), este debe ser un campo común en las tablas relacionadas que, si no existe, se debe crear
Con esto es posible generar el esquema de nuestra tabla de datos relacional previo a su creación en el software SQL

#### Para poner aprueba esto, se diseña un prototipo de base de datos relacional para películas a modo descriptivo identificando sus relaciones (uno a uno, uno a muchos o muchos a uno; muchos a muchos, si bien es posible, se evita o se reorganiza de forma que quede como una de las tres relaciones anteriormente enumeradas).


