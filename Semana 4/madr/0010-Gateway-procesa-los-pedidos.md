# Decisión de Diseño ADD-10: Hacer que el gateway procese los pedidos
 
 
* Status: rejected
* Deciders: Antonio Agudo Esperanza
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
* Chosen option: Crear un microservicio que procese los pedidos (ver [ADD-0011](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/Semana%204/madr/0011-Implementar-el-procesado-de-pedidos-como-un-microservicio.md))
## Positive Consequences
* Es más sencillo de desarrollar
## Negative Consequences
 * ya que se está añadiendo funcionalidades que no corresponden al gateway
 * ya que si hay mucho pedidos el gateway podría retrasarse en sus otras tareas
## Pros and Cons of the Options
Crear un microservicio que procese los pedidos
* Bueno, se quita carga del gateway
* Bueno, se mantiene una arquitectura modularizada
* Malo, puede resultar más complicado de desarrollar
 
## Links <!-- optional -->

* [Requisito funcional 001.1](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
