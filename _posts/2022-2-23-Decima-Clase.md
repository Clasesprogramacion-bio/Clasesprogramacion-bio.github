---
layout: post
title: DÉCIMA CLASE
---
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Resumen HTML y CSS</title>
    <link rel="stylesheet" href="styles.css" />
  </head>
  <body>
    <h1>Resumen de clase 19/02/2022</h1>
    <h2>HTML y CSS</h2>
    <p>
      En la clase del 19 de febrero, aprendimos que la estructura basica de HTML que se trabajara en el curso será html:5, y está dividido principalmente de 4 partes
    </p>
    <ul>
      <li>
        <strong>DOCTYPE</strong> , en donde se le especifica que tipo de comento se tratará
      </li>
      <li>
        <strong>hmtl lang=""</strong> , en donde se especifica que lenguaje regirá nuestra paguina web
      </li>
      <li>
        <strong>head</strong> , En donde se pone informacion metadata del sistema que como el tipo de caracteres que se usarán (UFT-8), titulo de la paguina y conexiones que esta peuda tener con otras ventanas
      </li>
      <li>
        <strong>body</strong> , Donse se añarira la informacion que será vista por el usuario
      </li>
    </ul>
    <br />
    <p>
      Tambien aprendimos de nociones basicas del sistema que añade contenido a una paguina
    </p>
    <p>Los comandos basicos aprendidos en HTML fueron los siguientes:</p>
    <ul>
      <li>
          La etiqueta "h#" ingresa un titulo, dependiendo del numero ingresado (De 1 a 6) da importancia al titulo, siendo 1 el mas notorio y reduciendo su tamaño de fuente a medida que el numero incrementa
      </li>
      <li>
          La etiqueta "p" nos ayuda a ingresar parrafos al sistema
      </li>
      <li>
          La etiqueta "ol" nos permite ingresar listas ordenadas numericamente
      </li>
      <li>
          La etiqueta "ul" nos permite ingresar listsas sin orden especifico
      </li>
      <li>
          La etiqueta "dl" permite crear una lista descriptiva
      </li>
      <li>
          Las imagenes se cargan mediante la etiqueta "img" y añadiendo la direccion de la imagen de la siguiente manera "src = 'dirrecion_imagen'"
      </li>
      <li>
          Los enlaces se generan mediante la etiqueta "a" y añadiendo la direecion de la imagen de la siguiente manera "href = 'direccion_link'"
      </li>
      <li>
          La etiqueta "div" permite genera una estructura de bloque
      </li>
      <li>
          La etiqueta "span" permite generar una estructura en linea
      </li>
    </ul>
    <br />
    <p>
        Aprendimos tambien que mediante CSS podemos decorar o modificar el aspecto de todos y cada uno de los componente anteriores, usando un documento diferente generalmente deniminadoo "styles.css" y definiendo los elements a modificar segun su nombre general ("p", "ul", "div", etc) o declarando un nombre unico para cada componente añadiendo un parametro "class = 'nombreObjeto'" y llamandolo mediante ese nombre en documento css. Todos los elementos llamadas se les modificará su apariencia tratando su parametros en modo JSON en donde cada llave corresponde a una caracteristica a modificar.
    </p>
    <dl>
        <dt><strong>color:</strong></dt>
        <dd>
            Modifica el color de la letra del objeto mediante el metodo rgba(#, #, #, #) o hexadecimal, en donde se les especifica la el color que se dese y la transparencia que se desee aplicar
        </dd>

        <dt><strong>font-size:</strong></dt>
        <dd>
            Modifica el tamaño de la letra del objeto
        </dd>

        <dt><strong>text-align</strong></dt>
        <dd>
            Modifica la distribucion del tecto
        </dd>

        <dt><strong>font-weight</strong></dt>
        <dd>
            Especifica el grueso de la linea
        </dd>
    </dl>

  </body>
</html>
