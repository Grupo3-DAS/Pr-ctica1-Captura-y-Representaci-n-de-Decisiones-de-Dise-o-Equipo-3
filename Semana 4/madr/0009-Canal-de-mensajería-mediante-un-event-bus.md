
# Decisión de Diseño ADD-09: Canal de mensajería mediante un event bus
* Status: proposed
* Deciders: Antonio Agudo Esperanza
* Date: 2020-12-01
## Context and Problem Statement
* La lógica de aplicación deberá contener un canal de mensajería para que se comuniquen los diferentes microservicios entre ellos. Este deberá estar basado principalmente en agentes de mensajes.
## Decision Drivers
* Los microservicios deberán comunicarse entre ellos
* El cliente requiere una implementación del bus de eventos
* La mensajería debe ser asíncrona
## Considered Options
* Bus de eventos
* Publish and Subscribe
## Decision Outcome
* Chosen option: Bus de eventos ya que permite un procesamiento sencillo de eventos y permite procesar un mismo evento por varios microservicios.
### Positive Consequences
* Permite procesar un mismo evento por varios microservicios.
* Se desvincula cada microservicio de los eventos
* Hay un sistema de comunicación general que facilita añadir nuevos microservicios
* Alta escalabilidad
### Negative Consequences
* Se tiene que agregar un subsistema para garantizar la entrega del evento.
## Pros and Cons of the Options
### Publish and Subscribe

* Bueno, ya que se puede realizar una implementación propia.
* Malo, ya que hay que definir métodos específicos para cada microservicio.
* Malo, ya que puede producir ralentizaciones
* Malo, porque puede producir sobrecargas.
## Links <!-- optional -->

* [Requisito RF002 y RF002.2](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
