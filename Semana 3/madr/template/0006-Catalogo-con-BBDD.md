# Usar BBDD para mostrar un catálogo de microservicios

* Status: proposed 
* Deciders:Antonio Agudo Esperanza y Marcos Robles Rodriguez
* Date: 2020-11-25


## Context and Problem Statement

Se requiere la funcionalidad de que haya un catálogo de microservicios.

## Decision Drivers <!-- optional -->

* Se quiere que simplemente sea un catálogo simple compuesto, por ejemplo, por una id, el nombre, una descripción corta y su URL.

## Considered Options

* AD007- Patrón composite

## Decision Outcome

Chosen option: Al final hemos seleccionado esta decisión ya que cumple con el requisito, y la otra opción hacía que los microservicios fueran dependientes del catálogo, por lo que provocaría dependencias innecesarias.

### Positive Consequences <!-- optional -->

*Es fácil añadir nuevos microservicios ya que solo es crear una nueva entrada en la base de datos.
*Es fácil de implementar.
*Es eficiente en memoria.


### Negative Consequences <!-- optional -->

* Puede resultar demasiado simple si se desea tener una descripción o campos detallados.

## Pros and Cons of the Options <!-- optional -->

### [option 1]

AD007- Patrón composite
 
Buena, agrupación de todos los microservicios en un único catalogo global
Mala, parentesco con una arquitectura monolítica