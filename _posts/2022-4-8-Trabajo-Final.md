---
layout: post
title: TRABAJO FINAL BACKEND
---
## INTRODUCCIÓN:
El Backend, justo con el Frontend y las bases de datos constituye un componente básico esencial en cualquier página WEB o software, esta entidad es la encargada
del procesamiento de la información que funciona como una "caja negra" para el usuario de la interfaz, a diferencia del Frontend, accediendo a la información contenida
en datos y realizando su procesamiento.

Para esta comunicación existen distintos protocolos de comunicación entre servidores WEB y navegadores entre los que se destaca el HTTP (Hypertext Transfer Protocol) que puede o no, ser seguro (HTTPS) que, siguiendo el modelo cliente-servidor.

## GET, PUT, POST, PATCH, UPDATE, DELETE & CRUD Methods:

So algunos de los métodos más comunes y coinciden con los empleados anteriormente en bases de datos puesto que permiten crear nuevos registros, leerlos, actualizarlos, modificarlos y eliminarlos, siendo de forma general y en esencia lo mismo que los métodos CREATE, READ, UPDATE, DELETE.

### HTTP Responses:
Algunas de las respuestas que podemos encontrar al ejecutar una acción que se realice mediante backend son:
- 100 Continue
- 101 Switching Protocols
- 103 Early Hints
- **200 OK** *más común*
- 201 Created
- 202 Accepted
- 203 Non-Authoritative Information
- 204 No Content
- 205 Reset Content
- 206 Partial Content
- 300 Multiple Choices
- 301 Moved Permanently
- 302 Found
- 303 See Other
- 304 Not Modified
- 307 Temporary Redirect
- 308 Permanent Redirect
- 400 Bad Request
- 401 Unauthorized
- 402 Payment Required
- 403 Forbidden
- 404 Not Found
- 405 Method Not Allowed
- 406 Not Acceptable
- 407 Proxy Authentication Required
- 408 Request Timeout
- 409 Conflict
- 410 Gone
- 411 Length Required
- 412 Precondition Failed
- 413 Payload Too Large
- 414 URI Too Long
- 415 Unsupported Media Type
- 416 Range Not Satisfiable
- 417 Expectation Failed
- 418 I'm a teapot
- 422 Unprocessable Entity
- 425 Too Early
- 426 Upgrade Required
- 428 Precondition Required
- 429 Too Many Requests
- 431 Request Header Fields Too Large
- 451 Unavailable For Legal Reasons
- 500 Internal Server Error
- 501 Not Implemented
- 502 Bad Gateway
- 503 Service Unavailable
- 504 Gateway Timeout
- 505 HTTP Version Not Supported
- 506 Variant Also Negotiates
- 507 Insufficient Storage
- 508 Loop Detected
- 510 Not Extended
- 511 Network Authentication Required
El presente trabajo tiene como propósito integrar lo aprendido a lo largo del curso de Programación WEB respecto al diseño de una página de internet que brinde servicio de agendamiento y seguimiento de citas médicas guardando información relacionada con el personal médico profesional, los usuarios en calidad de paciente y una reseña de su historial en citas médicas cuyo desarrollo Frontend y registro/implementación de bases de datos fue llevado a cabo en anteriores trabajos, por lo que este escrito se interezará en la exploración del desarrollo Backend que permitirá la comunicación "detrás" de la página con el servidor.


---------------------------------------
## METODOLOGÍA:
En una imagen de Vagrant y usando Docker como plataforma contenedora y haciendo uso de Python con su módulo Flask, se desarrollarán las funciones pertinentes para los distintos métodos CRUD en la base de datos (MongoDB) del servidor WEB, esto para poder manipular los datos de pacientes y sus respectivas citas médicas dados los datos fijos de médicos y hospitales, para ello, como se evidenciará en el código, se Crearán, leeRán, actUalizarán y Descartarán campos de datos referidos a estas colecciones mencionadas.

También se utilizará *POSTMAN* una herramienta de fácil uso y altamente útil para el desarrollo backend en la verificación de la ejecución de estos métodos observando la respuesta HTTP/1.1 que genere la interacción con la WEB.


<img src="{{ site.baseurl }}/images/createpaciente.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/createpostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestacreatepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/readpaciente.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/readpostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestareadpostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/updatepaciente.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/updatepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestaupdatepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/deletepaciente.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/deletepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestadeletepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/createmedico.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/createpostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestacreatepostman.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/readmedico.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/readpostmanmed.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestareadpostmanmed.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/updatemedico.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/updatepostmanmed.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestaupdatepostmanmed.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/deletemedico.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/deletepostmanmed.jpeg" style="width: 480;"/>


<img src="{{ site.baseurl }}/images/respuestadeletepostmanmed.jpeg" style="width: 480;"/>
---------------------------------------
## CONCLUSIONES:
- A
- B
- C


---------------------------------------
## REPOSITORIO
[github](/site)
