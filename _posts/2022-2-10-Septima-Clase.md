---
layout: post
title: SÉPTIMA CLASE
---
## BASES DE DATOS NO RELACIONALES (NO-SQL DATABASE):
Culminada la unidad de JAVASCRIPT, se explica su importancia para la unidad siguiente que el de bases de datos no relacionales, se inicia la clase definiendo estas últimas con un breve repaso de su historia y diferenciándolas de las bases de datos de tipo SQL junto con algunos conceptos generales importantes para entender su manejo.

### ¿Qué es una base de datos no relacional?
Su aplicación se basa en el de cualquier base de datos pero se diferencia en cuanto a que no hay integridad de la información a partir de la relación.

### Schema-Less:
No hay una estructura definida de datos, estos se pueden grabar arbitrariamente ya que su definición se realiza mediante registros. La gestión de la estructura de datos se traslada a la aplicación.

### Tipos de estructuras en bases de datos no relacionales:
* Clave-valor
* Documentos
* Grafos
* Column family
* En memoria
* Cualquier tipo de almacenamiento que no use relaciones para mantener la consistencia de los datos

### Algunas ventajas que ofrece respecto a las SQL:
Son fáciles de usar, flexibles, no utilizan lenguaje declarativo de consulta, son óptimas para gestión de mayor cantidad de datos, son altamente escalables; esto se refiere a la capacidad de crecer y seguir funcionando bien, se consideran de rápido desarrollo.

### Definición de bases de datos documentales:
Colección que contiene cada ítem como documento (XML, JSON) que describe su propia estructura de datos consultados por campos específicos incluyendo diferentes tipos de datos.
{imagen}

#### JSON (JavaScript Object Notation):
Es un formato de alto nivel e intepretado, ideal para intercambio de datos, hace parte de un subconjunto del lenguaje JavaScript construido por pares {“conjunto”:”valor”,}
#### YAML (Yet Another Markup Language):
Formato de aún mayor nivel que puede ser incluso intuitivo para personas sin experiencia en programación pues su sintaxis se parece al de la escritura en un cuaderno remplazando tabulación por espacios, listas indicadas por guiones al mismo nivel de identación, eliminando uso de comillas y otros símbolos gramaticales como paréntesis, corchetes y llaves.

### Ejemplo de aplicación de base de datos no relacional estructura JSON y YAML
Se dearrolló el mismo ejemplo de una base de datos de películas utilizando JAVASCRIPT en el entorno VisualStudio Code evidenciando su forma de aplicación general y diferencias repecto al ejemplo anteriormente desarrollado en MySQL.

