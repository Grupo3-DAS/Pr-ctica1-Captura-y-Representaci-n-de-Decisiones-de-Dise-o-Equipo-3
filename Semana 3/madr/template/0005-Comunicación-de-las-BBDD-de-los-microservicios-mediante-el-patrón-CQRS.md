# Decisión de diseño ADD-05: Comunicación de las BBDD de los microservicios.
* Status: proposed
* Deciders: Antonio Agudo Esperanza y Marcos Robles Rodríguez
* Date: 2020-11-24
## Context and Problem Statement
* Se debe comunicar las distintas BBDD con sus microservicios.
## Decision Drivers
* División de comandos y queries
* Sugerencia del cliente
## Considered Options
*  Mediante acceso directo
## Decision Outcome
* Chosen option: "Comunicación de las BBDD de los microservicios mediante el patrón CQRS, ya que opinamos que dividir las operaciones en dos subgrupos puede ayudar a que haya menos congestión, como por ejemplo, si hay muchas queries y pocos comandos, que los comandos no tengan que esperar.
## Positive Consequences
* Separación de responsabilidades
* Evitar la congestión en una operación concreta si esta está poco cargada.
## Negative Consequences
* Complejidad del código
* Coherencia: Si separas la lectura de la escritura puede darse el caso de que al leer la información de la base de datos, puede estar desactualizada.
## Pros and Cons of the Options
### Mediante acceso directo
* Bueno, ya que es mucho más simple.
* Bueno, ya que siempre se va a leer información actualizada.
* Mala, ya que hay mucha más congestión.

 
## Links <!-- optional -->
* [Requisito RF005](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
* [Información de](https://martinfowler.com/bliki/CQRS.html) <!-- example: Refined by [ADR-0005](0005-example.md) -->

