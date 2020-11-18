# El sistema constará de un servicio de gestión de solicitudes y respuestas y se usa usa una arquitectura cliente-servidor

* Status: proposed
* Deciders: Antonio Agudo y Marcos Robles
* Date: 2020-11-17

## Context and Problem Statement

  Comunicación con el cliente por solicitudes y respuestas
  
## Decision Drivers <!-- optional -->

* El sistema debe comunicarse con los clientes mediante solicitudes y respuestas, por lo que se sugiere que actúen como cliente servidor

## Considered Options

* Cliente-servidor
* Peer to Peer

## Decision Outcome

Chosen option: Cliente-servidor, ya que es la idea principal que se adapta a todas las necesidades cuando se piensa en intercambio de datos.

### Positive Consequences <!-- optional -->

* Mucho Control sobre el tráfico
* Centralización del control
* Fácil mantenimiento
* Segura
* Poco coste de recursos para el cliente
* Puede funcionar sin clientes

### Negative Consequences <!-- optional -->

* Congestión del tráfico
* Poca robustez en caso de fallo comparado con P2P
* El software y el hardware del servidor aumentará el costo
* El servidor contiene la aplicación, si este falla todos los clientes fallarán.

## Pros and Cons of the Options <!-- optional -->

### Peer to Peer

Red distribuida de datos

* Bueno, porque, al igual que los microservicios, tiene una gran escalabilidad
* Bueno, porque, descongestiona el tráfico con el servidor
* Bueno, porque aporta mayor robustez
* Bueno, porque tiene una mayor velocidad
* Malo, porque requiere que haya un número mínimo de usuarios para trabajar
* Malo, porque no permite un control centralizado
* Malo, porque la presencia de firewalls o proxys puede dificultar que el usuario use el sistema
* Malo, porque cada microservicio una base de datos puede resultar ineficiente en memoria para el cliente, y puede haber redundancia, o puede darse que se hayan desconectado de la red todos los clientes con ese dato y no esté disponible 


