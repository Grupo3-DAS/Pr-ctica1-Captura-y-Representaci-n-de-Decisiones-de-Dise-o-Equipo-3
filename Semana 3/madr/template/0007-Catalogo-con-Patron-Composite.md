# Decisión de Diseño ADD-0007: Uso del patrón Composite para mostrar los microservicios

* Status: rejected
* Deciders:Antonio Agudo Esperanza y Marcos Robles Rodriguez
* Date: 2020-11-25

Esta decisión se hizo de manera paralela a la ADD-0006

## Context and Problem Statement

Para mostrar los diferentes tipos de microservicios he propuesto usar el patrón composite para acceder a cada uno de los microservicios.

## Decision Drivers <!-- optional -->

* Agrupación de los microservicios en un único catálogo


## Considered Options

* AD006-Uso BBDD

## Decision Outcome

* Chosen option: Esta opción ha sido rechazada, mirar AD006

### Positive Consequences <!-- optional -->

* Agrupación de todos los microservicios en un único catalogo global

### Negative Consequences <!-- optional -->

* Parentesco con una arquitectura monolítica

## Pros and Cons of the Options <!-- optional -->

### Uso BBDD

* Bueno, ya que es fácil añadir nuevos microservicios ya que solo es crear una nueva entrada en la base de datos.
* Bueno, porque es fácil de implementar.
* Bueno, ya que es eficiente en memoria.
* Malo, porque puede resultar demasiado simple si se desea tener una descripción o campos detallados.

## Links <!-- optional -->

* [Requisito RF004](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
