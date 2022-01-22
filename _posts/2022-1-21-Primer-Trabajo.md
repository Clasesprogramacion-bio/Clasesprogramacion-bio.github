---
layout: post
title: PRIMER TRABAJO
---
## INTRODUCCIÓN:
La aparición de las herramientas informáticas ha facilitado muchas funciones cotidianas y de labor científica, además de representar ventajoso en cuanto a comunicación y seguridad
de la información, en el caso concreto de las bases de datos virtuales, han evolucionada hasta el punto de permitir almacenar una gran cantidad de información haciendo fácil y 
seguro su acceso y registro en comparación con métodos más arcaicos que en su mayoría incluían gasto de abundante papel con el riesgo inminente de pérdida de información debido 
a humedad, envejecimiento e incendios, además de la claramente tediosa tarea que representaba la búsqueda y filtrado de los datos almacenados de esta forma. 

La pandemia declarada por la COVID-19 ha acelerado la transición a modalidades virtuales en todos los campos que se pueda imaginar, siendo de especial relevancia el médico. 
Un logro de esto es la telemedicina que, si bien data desde hace casi un siglo (las primeras consultas médicas realizadas por vía telefónica) [1], es cada día más relevante debido a la agilidad, comodidad, ahorro en tiempo y dinero que supone para los usuarios y, principalmente, la cobertura de este servicio que puede extenderse a zonas periféricas de reducido e incluso inexistente acceso a la medicina por otros medios haciéndose hincapié en su necesidad para algunos países en vía de desarrollo que carecen de la infraestructura y cultura necesaria para llevarla a cabo [2]. 

El presente trabajo pretende por medio de software crear una plataforma que permita, en una fase inicial, el agendamiento y seguimiento de citas médicas que busca beneficiar a los usuarios del sistema médico tanto en su rol de practicantes como de pacientes a fin de facilitar la gestión de información.


---------------------------------------


## METODOLOGÍA:
Inicialmente, y a modo de apoyo, se diseñará un boceto inicial que indique la relación existente entre los datos que se manejarán; esto facilitará su posterior configuración en el software gestor de bases de datos MySQL.


Se considerará inicialmente las variables que identifican el rol de la persona que accede al sistema de agendamiento de citas identificados por una clave primaria, según esto, 
se recopilará nombre, apellido y, según el motivo de la consulta o remisión profesional, se asignará una cita con un profesional especializado. De la cita se tendrá en cuenta el 
espacio y el tiempo en que tendrá lugar según sea el caso; del médico se considerará nombre, apellido y especialidad que posee; el hospital a su vez poseerá su nivel y la 
dirección en la que se ubica si se dará de forma presencial o de lo contrario se indicará que es virtual junto con el enlace de acceso, esto a fin de informar al usuario a 
dónde deberá remitirse para ser atendido.


---------------------------------------



## Diccionario de datos 
En el diagrama se observan las entidades y sus respectivas relaciones que se manejarán en la base de datos según el equipo de trabajo lo consideró necesario:


![Diagrama](images/diag.jpeg)


Con el fin de conocer los componente del proceso, a continuación se hará una breve descripción de los mismos:
### Entidades
#### Paciente
Esta tabla contiene la información relevante que será tomada del paciente.


**ID:** Identificación única y propia con la que se distinguirá de otros pacientes
	
	
**Nombre:** Nombre del pacientes
	
	
**Apellido:**  Apellido del paciente
	
	
**ID Medico:** Identificación del médico al que será adscrito
	
	
**ID Cita:** Identificación de la cita 


#### Cita
Esta tabla contendrá información relevante de la cita que el paciente tendrá 


**ID:** Individualización de cita para seguimiento posterior en caso de que sea necesario.  
	
	
**ID Paciente:** Paciente a quien fue agendada la cita
	
	
**ID Medico:**  Médico que atenderá la cita
	
	
**Estado:** Indica la vigencia de la cita al momento de la consulta
	
	
**Fecha:** Fecha en que se llevará a cabo la cita 
	
	
**Hora:** Hora del día en que fue agendada la cita
	
	
**ID Hospital:** Hospital en el que se llevará a cabo la cita agendada 
	
	
**Costo:**  Depósito que deberá cancelar el paciente 
	

#### Prescripción
Esta tabla contiene información clave para el tratamiento que deba seguir el paciente. 


**ID:** Identificación de prescripción que fue dada a un paciente, en una cita específica. 
	
	
**Posología:** Cuidados y recomendaciones que el paciente deberá seguir para su pronta recuperación
	
	
**Descripción:** Prescripción médica en donde indica medicamentos, dosis y frecuencia de administración que el paciente debe seguir.
	

#### Medicamento
Esta tabla contendrá información sobre el medicamento que deberá tomar el paciente acorde a la prescripción que le fue dada


**ID:** Identificación del medicamento.
	
	

**Nombre:** Nombre mediante el cual pueda ser adquirido en farmacias u hospitales. 
	
	
#### Médico
Esta tabla contiene información relevante del médico que atendió la cita de un paciente y que posteriormente realizará una prescripción médica.
	
	
**ID:** Clave primaria que distingue al profesional médico que atenderá la cita
	
	
**Nombre:** Nombre del médico
	
	
**Apellido:** Apellido del médico
	
	
**ID Cita:** Identificador de las citas que estará atendiendo el médico
	
	
**Especialidad:** Área de enfoque clínico del médico
	
	
#### Hospital
Esta tabla recoge los datos principales del lugar donde se llevará a cabo la consulta médica
	
	
**ID:** Código de identificación del hospital
	
	
**Nivel:** Grado de gestión clínica característica de un hospital
	
	
**Dirección:** Ubicación exacta del ente donde se llevará a cabo la cita médica

### Relaciones
#### Prescripción-medicamento
Esta tabla describe la información compartida entre la tabla de prescripción y la de medicamento.
	
	
**ID prescripción:** Clave primaria que indica la receta hecha por el médico
	
	
**ID medicamento:** Identificador de los medicamentos que se incluyen en la prescripción.


#### Médico-hospital
Esta tabla describe la información compartida entre la tabla de médico y la tabla hospital. 
	
	
**ID médico:** Clave primaria de los médicos que se encuentran en este hospital
	
	
**ID hospital:** Índice del hospital


---------------------------------------



## Conclusiones:
*	Para poder realizar una base de datos óptima, es necesario tener claro los conceptos que se derivan de los datos que se manejarán, teniendo un buen nivel de manejo del área
al que se apunta, es más fácil definir las entidades y las relaciones que existen entre estas.
*	Con un correcto esquema de diseño previo de la base de datos, es más fácil entrar en materia de construcción en Software y también es fácil luego la manipulación de los datos
en la programación del filtrado, búsqueda y alimentación de la información.
*	La digitalización de la información facilita su manipulación, además de brindar seguridad y estabilidad difícilmente lograda con el archivo de recursos físicos.


---------------------------------------



## Referencias:
⋅⋅⋅[1] https://clinic-cloud.com/blog/historia-de-la-telemedicina/
⋅⋅⋅[2] https://larepublica.es/2020/09/04/la-importancia-de-la-telemedicina-en-nuestros-dias/

