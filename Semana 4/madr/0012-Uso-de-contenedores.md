# Decisión de Diseño ADD-12: Elección de contenedor de nuestros microservicios
* Status: proposed
* Deciders: Antonio Agudo Esperanza y Marcos Robles Rodriguez
* Date: 2020-12-02 
## Context and Problem Statement
* Necesitamos usar un contenedor para guardar todos los microservicios y todo lo necesario para la parte del servidor de nuestra arquitectura, con Docker
# Decision Drivers
* Que los contenedores estén modularizados
* Escalabilidad
 
## Considered Options
* Usar docker host
## Decision Outcome
* Chosen option: Docker ya que permite buena escalabilidad y está preparado para ejecutarse rápidamente
### Positive Consequences
* Mejora continua
* Implementación rápida
* Capacidad de restaurar a una versión anterior del microservicio
* Modularidad
### Negative Consequences
* Problemas de seguridad
## Links <!-- optional -->

*  [Requisito funcional 002.1.1](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf)
