[![Build Status](https://travis-ci.org/i4vk/GymManager.svg?branch=master)](https://travis-ci.org/i4vk/GymManager) [![Run Status](https://api.shippable.com/projects/5d9ca4ed27d7a0000752c711/badge?branch=master)]() [![Coverage Status](https://coveralls.io/repos/github/i4vk/GymManager/badge.svg?branch=master)](https://coveralls.io/github/i4vk/GymManager?branch=master)

# GymManager

## Gestor de usuarios y empleados de un gimnasio

La idea es crear una API que permita manejar una base de datos en la cual se podrán almacenar datos de los clientes suscritos al gimnasio, los cuales podrán tener además distintas tarifas cada uno. Por ejemplo, clientes completos, con acceso al gimnasio todos los días de la semana, o clientes básicos, con acceso un número de días limitado.

De dichos clientes se almacenarán distintos datos que podrían ser útiles, como son por ejemplo del nombre completo, el teléfono, el DNI, y el número de socio, que será único para cada uno de los clientes. También será importante almacenar la tarifa asociada a dicho cliente.

## Funcionalidades

Este microservicio formaría parte de una aplicación completa que maneje el sistema informático completo de un gimnasio, tales como los accesos al gimnasio, el registro de clientes, etc.

Sin embargo, la funcionalidad de este microservicio que vamos a desarrollar durante la asignatura va a encargarse únicamente de manejar la base de datos de clientes.  
Para llevar a cabo esta función, debe disponer de las siguientes funcionalidades:

  - Crear una nueva base de datos de clientes.
  - Añadir un nuevo cliente a la base de datos.
  - Modificar los datos de alguno de los clientes ya creados.
  - Eliminar clientes de la base de datos.
  - Consultar la lista completa de clientes.
  - Consultar los datos de un cliente específico.

## Implementación

Las herramientas utilizadas para llevar a cabo el proyecto serán las siguientes:

  - Lenguaje de programación: **Javascript**.  
  Más concretamente, usaremos *Node.JS*, que es un entorno de ejecución para desarrollar con javascript en el lado del servidor.

  - Framework de aplicaciones web: **ExpressJS**.  
  Es el framework más usado sobre *nodejs* para trabajar con el protocolo http y para tener un sistema de rutas que nos permitirá implementar nuestra *API RESTful*.

  - Base de datos: **MongoDB**.
  Se usará una base de datos para almacenar toda la información de los clientes de forma permanente. En este caso, he decidido usar MongoDB, que es una base de datos NoSQL que nos permitirá llevar a cabo todas las tareas relacionadas con dicha base de datos.

  - Sistema de logs: **Morgan**.  
  Es importante mantener un registro de logs que vayan indicando qué está ocurriendo en cada momento en nuestro sistema. Si hay algún fallo, esto permite saber por ejemplo qué es lo que ha pasado, y dónde ha fallado exactamente.  
  En este caso, he decidido utilizar la biblioteca *Morgan*.

  - Test: **Jest**.  
  Es necesario comprobar el correcto funcionamiento de nuestros programas antes de poder desplegarlos, para así tener la certeza de que aquello que desplegamos hace correctamente la función que le ha sido encomendada.  
  Para ello, vamos a utilizar la biblioteca *Jest*, que nos permite justamente realizar test que todo lo que implementemos deberá ser capaz de pasar, antes de poder ser desplegado.

  - **Travis-CI** para la integración continua.

## Documentación

*Coming soon.*

## Instalación

*Coming soon.*
