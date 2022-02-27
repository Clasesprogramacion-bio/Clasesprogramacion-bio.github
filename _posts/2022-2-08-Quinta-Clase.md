---
layout: post
title: QUINTA CLASE
---
### JAVASRIPT I
esto es un post
# desarrollo frontend 1
### cuales son las tecnologías principales para frontend?
- html, css, javascript
### qué rol toma cada una de esas tecnologías?
- html: define la organización del contenido de la página, en qué parte va cada elemento
- css: se encarga del aspecto estético de la página, tamaños, colores, posiciones, fuentes, etc.
- javascript: se encarga de aspectos lógicos de la página como resolver cálculos, mandar alertas,
traer información de otros dominios, etc.
### fundamentos de javascript
#### como llamar código de javascript desde el navegador?
- simplemente debe colocarse la siguiente etiqueta:
`<script src="js/rutaArchivoJs.js"></script>`
- en el documento html que se esté abriendo en el navegador.
#### inicializacion de variables en javascript
- `var variable = 1`
- las variables definidas con `var` tienen un alcance global, esto significa
que pueden ser llamadas desde cualquier parte del código.
- `let variableBloque = 1`
- las variables definidas con `let` tienen un alcance local, es decir que el valor de la variable definida con let solo puede ser accedido en el bloque en el que se encuentra o bloques hijos y no en bloques no relacionados.
- `const constante = 1`
- las "variables" definidas con `const` tienen el mismo alcance que las variables definidas con let, pero no pueden ser modificadas.
- en general se recomienda definir las variables con `let` ó `const` para limitar el alcance (scope) de las variables y no definir variables globales que se modifiquen de manera involuntaria posteriormente.
#### tipos de datos primitivos
- Bolean: true, false, los datos bolean se utilizan para el flujo de las aplicaciones y pueden ser
el resultado de operaciones de comparación, los datos no vacíos a excepción del 0 se toman como verdaderos
y los datos vacíos y no definidos y el 0 se toman como verdaderos
- null: tipo de dato nulo que se usa para referenciar referencias inexistentes o para inicializar variables
- Undefined: dato asignado a las variables que no se han definido o inicializado.
- Number: dato utilizad para representar números entre 
 -(2^53 - 1) y 2^53 -1, los valores especiales del number son +Infinity y -Infinity que representan un número mayor y menor a todos los demás respectivamente y NaN para expresar que el resultado de una operación no retornó un entero, ej: división por 0
- BigInt: permíte almacenar números enteros grandes con una cierta precisión.
- symbol: tipo de dato inmutable que se puede usar como llave de objetos
- String: utilizado para representar caracteres
#### objetos
- tipo de dato compuesto por pares de keys y values qué permite almacenar estructuras complejas en una misma variable, por ejemplo:
- `let objeto = {
    nombre: "alexander",
    apellido: "garcia",
    edad: 25,
    mayorDeEdad: true
}`
- los objetos permiten almacenar diferentes tipos de datos, por ejemplo en el ejemplo anterior el objeto guarda Strings, Numbers y Boolean.
#### operaciones de comparación:
- permiten realizar comparaciones entre elementos.
- `a > b`: evalua si la variable `a` es mayor a la variable `b`, en ese caso devuelve `true`, en caso contrario devuelve false
- `a >= b` el resultado es `true` si `a` es mayor o igual a b, en otro caso el resultado es `false`.
- otras operaciones son
- `a < b`
- `a <= b`
- `a == b`: verifica igualdad de valores, por ejemplo `1 == "1"` es verdadero
- `a === b`: verifica igualdad de valores y de tipos, por ejemplo 
#### operaciones de comparacion
- `a && b`: devuelve `true` si `a === true` y `b === true`, en otro caso devuelve `false`
- `a || b`: devuelve `false` si `a === false`
- `!a`: devuelve `false` si `a === true` o `true` si `a === false`
- como se mencionó antes, el `0`, `null` y `undefined` son intercambiables por `false` y datos no vacíos
diferentes de `0` ó  `false` son intercambiables por `true` en las operaciones de comparación.
#### control de flujo
- utilizan valores boleanos para decidir qué partes del código ejecutar, el el siguiente ejemplo, la porción del código "1" se ejecutará si `condicion1 === true`
la porción del código "2" se ejecutará si `condicion2 === true`, la porcion del código "n" se ejecutará si `condicionN === true` y en otro caso se ejecutará la porción
del código "en otro caso" en el bloque `else`
`
if(condicion1){
    // codigo 1
}
else if(condicion2){
    // codigo 2
}
...
else if(condicionN){
    // codigo "n"
}
else{
    // en otro caso
}
` 
- al igual que para las operaciones de comparación, el `0`, `null` y `undefined` son intercambiables por `false` y datos no vacíos
diferentes de `0` ó  `false` son intercambiables por `true` estructuras de control de flujo.
