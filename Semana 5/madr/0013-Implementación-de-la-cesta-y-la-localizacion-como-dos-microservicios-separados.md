# Implementación de la cesta como un microservicio y las localizaciones de terceros
* Status: proposed
* Deciders:Antonio Agudo Esperanza y Marcos Robles Rodriguez
* Date: 2020-12-08
## Context and Problem Statement
* Se pide implementa una cesta de la compra que usará una caché y la localización de microservicios de terceros en MongoDB 
## Decision Drivers
* Se nos pide implementar la cesta.
* Se píde que la cesta use una cache
* Queremos que la arquitectura siga lo más modularizada posible
* Se supone que la localización de microservicios va asociada a la cesta.
* Se pide que la localización de microservicios de terceros tenga una base de datos en MongoDB
## Considered Options
* Usar una Caché e implementar en el microservicio la búsqueda de localizaciones de terceros de manera interna
* Crear un microservicio que se encargue de buscar localizaciones de terceros con MongoDB y otro microservicio con una caché interna que implemente las funcionalidades de la cesta
## Decision Outcome
* Chosen option:  Implementaremos el nuevo microservicio por separado ya que esto nos permitirá seguir con la modularidad y además, en el caso de que otro microservicio necesite la localización de terceros ya no tendremos que volver a  desarrollarlo
### Positive Consequences
* Se mantiene la modularidad.
* Reutilización de microservicios
* Escalabilidad
### Negative Consequences
* Complejidad a la hora de hacerlo.
* Probabilidad de exceso de mensajes en el bus de eventos.
## Pros and Cons of the Options
### Usar una Caché e implementar en el microservicio la búsqueda de localizaciones de terceros de manera interna
* Bueno, ya que el acceso es más rapido
* Bueno, ya que la creación va a ser más rápida 
* Malo, ya que la localización no se puede reutilizar
* Malo, ya que no se respeta la modularidad

## Links <!-- optional -->

*  [Requisito funcional 007](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
