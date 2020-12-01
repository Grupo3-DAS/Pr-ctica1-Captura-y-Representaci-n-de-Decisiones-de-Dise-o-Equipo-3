# Uso de un gateway a diferentes APIs
* Status: proposed <!-- optional -->
* Deciders: Antonio Agudo Esperanza y Marcos Robles Rodríguez<!-- optional -->
* Date: 2020-12-1 <!-- optional -->

## Context and Problem Statement

El cliente nos ha expuesto que usemos un gateway y hemos decidido conectarlo a unas API cada una con su microservicio para que sea posible una modularización óptima 

## Decision Drivers <!-- optional -->

* El cliente comenta el uso de una gateway
* Busqueda de completitud a la hora de comunicar cliente servidor
* Busqueda de la máxima modularidad por el uso de una API para cada microservicio

## Considered Options

* Uso de gateway
* Conexion directa entre el cliente con los microservicios

## Decision Outcome

Chosen option: Uso de el gateway, porque consideramos muy importante la modularización y el bajo acoplamiento para que sea posible una mejor escalabilidad en nuestra arquitectura, además, las APIs y el gateway puede realizar acciones intermedias como el procesamiento de pedidos y puede servir como una capa extra de seguridad.

### Positive Consequences <!-- optional -->

* Escalabilidad
* Modularidad
* Bajo acoplamiento
* Capa extra de seguridad
* Posibilidad de añadir funciones intermedias entre el cliente y el servicio

### Negative Consequences <!-- optional -->

* Mayor complejidad en la arquitectura y el código.

## Pros and Cons of the Options <!-- optional -->

### Cliente servidor directo>

* Bueno, ya que es más simple de programar y hacer.
* Malo, ya que el cliente debe conocer a la perfección los microservicios ya que no hay ninguna API que se los facilite
* Malo, porque no hay nada que se interponga entre una mala solicitud y los microservicios dejando un agujero de seguridad

## Links <!-- optional -->

* [Requisito Funcional 1.x](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
* … <!-- numbers of links can vary -->
