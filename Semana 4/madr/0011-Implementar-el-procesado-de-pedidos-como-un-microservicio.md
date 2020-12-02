# Decisión de Diseño ADD-11: Implementar el procesado de pedidos como un microservicio
* Status: proposed
* Deciders: Marcos Robles Rodríguez
* Date: 2020-12-02
## Context and Problem Statement
* Se pide que el sistema sea capaz de procesar los pedidos que le llegan.
## Decision Drivers
* Respetar la arquitectura de microservicios
* Quitar carga de partes del sistema que no sean un microservicio
## Considered Options
* Hacer que el gateway procese los pedidos
* Crear un microservicio que procese los pedidos
## Decision Outcome
* Chosen option: Implementaremos el nuevo microservicio por separado ya que esto nos permitirá seguir con la modularidad y así no le ponemos tareas adicionales al gateway
### Positive Consequences
* Se quita carga del gateway
* Se mantiene una arquitectura modularizada
### Negative Consequences
* Puede resultar más complicado de desarrollar
## Pros and Cons of the Options
### Hacer que el gateway procese los pedidos
Se pensaba que según le entraban las solicitudes al gateway este comprobara si era un pedido y lo procesara él.
* Bueno, ya que es más sencillo de desarrollar
* Malo, ya que se está añadiendo funcionalidades que no corresponden al gateway
* Malo, ya que si hay mucho pedidos el gateway podría retrasarse en sus otras tareas
## Links <!-- optional -->

* [Requisito funcional 001.1](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
