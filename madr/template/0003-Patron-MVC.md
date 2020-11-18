# Decisión de Diseño ADD-03: Se debe mostrar una interfaz de usuario
* Status:Proposed
* Deciders:Antonio Agudo y Marcos Robles
* Date:2020/11/18

## Context and Problem Statement
Se usará el patrón MVC para la comunicación con el cliente de los microservicios

## Decision Drivers
* Como se debe mostrar una interfaz al usuario, y esta debe tener los datos del microservicio, hemos decidido utilizar el MVC para que esté ordenado.

## Considered Options
* Patrón modelo-vista-controlador

## Decision Outcome
Chosen option: Hemos elegido el MVC ya que creemos que es una buena manera de tener la parte del diseño y el código de la interfaz bien ordenado.

## Positive Consequences
* Modularización
* Información actualizada siempre
* Las modificaciones en las vistas no afectan al modelo del dominio

## Negative Consequences
* Mayor dedicación en el desarrollo
