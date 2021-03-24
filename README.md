# Proyecto 1 - Tópicos de Telemática

El middleware tiene una gran importancia para la conexión de las aplicaciones, con otras
aplicaciones, procesos o servicios, en otras palabras, es ese puente que permite establecer la
comunicación y el paso de información para que los programas de software funcionen
correctamente. Con el objetivo de afianzar los conocimientos del middleware a través de la
práctica, se nos ha propuesto desde la materia Tópicos de Telemática de la Universidad
EAFIT, implementar un Middleware orientado a mensajes (MOM), donde tenemos clientes
publicadores que envían mensajes y otros consumidores que los reciben, dichos mensajes
pueden ser enviados y recibidos bajo un modelo de colas o canales, siendo el primero de ellos
el que reparte los mensajes entre los consumidores conectados, a manera de repartición de
tareas, y el segundo el que envía el mismo mensaje a todos los consumidores conectados en
el momento en que son enviados.

## Demo 🚀

Para utilizar la demo del proyecto, lo único que necesitas es descargar en tu máquina local, el archivo 
client.py en caso de que quieras ser un usuario publicador (envía mensajes gestionando colas y canales),
o consumidor.py en caso de que quieras ser un usuario consumidor (recibe mensajes conectándose a colas o canales)


### Pre-requisitos 📋

-Tener Python en tu máquina local.
-Importar los módulos de las clases que hayas descargado

### Instalación 🔧

Para tener una copia del proyecto en tu máquina local necesitas hacer los siguientes pasos:

-Descargar los archivos .py del repositorio. ***Ten en un cuenta que para correr el proyecto en tu máquina local 
vamos a cambiar el archivo Aplicacion.py, en lugar de este, vamos a descargar Aplicacion2.py, ya que nos permite
la encriptación de las claves de acceso a colas o canales exitosamente.***

-Cumplir con los pre-requisitos mencionados anteriormente.

-Si vas a correr el proyecto localmente, cambia la dirección IP tanto en client.py como en consumidor.py por 
"localhost" en la línea de conexión con sockets (línea 10 para ambos archivos).

-Ejecuta server2.py

-Ejecuta client.py y/o consumidor.py en nuevas consolas.


## Ejecución de pruebas ⚙️

Para probar el sistema sólo sigue el menú que aparece en pantalla al ejecutar client.py o consumidor.py.


## Detalles del proceso 🛠️

-***Análisis del proyecto:*** Todos los requerimientos fueron enfocados en cumplir con las funciones básicas 
de un Middleware orientado a mensajes, implementando tanto colas como canales, y velando por los atributos de calidad
más importantes de un middleware: seguridad, heterogeneidad, transparencia, disponibilidad y escalabilidad.

-***Diseño del proyecto:*** Fue muy enfocado en desarrollar una arquitectura que permitiera tener un proyecto escalable,
es por esto que el servidor MOM se montó en una máquina de AWS que nos provee los beneficios de la computación en la nube,
y los clientes los puede ejecutar cualquier persona desde su máquina local, con la posibilidad de lanzar varias consolas 
al mismo tiempo, en el documento "Diseño Proyecto 1.pdf" se encuentran más detalles de la arquitectura y el funcionamiento 
lógico tanto de colas como de canales.

-***Implementación del proyecto:*** Fue implementado en el lenguaje Python ya que es un lenguaje moderno que cada vez nos
ofrece más versatilidad a la hora de iniciar proyectos de desarrollo, nos ofrece un mejor manejo de estructuras de datos 
y algunas librerías que nos ayudaron a desarrollar mejor el proyecto.

## Autores ✒️

* **César Andrés García Posada**  
* **Daniel García García** 
* **Juan Camilo Guerrero Alarcón** 
