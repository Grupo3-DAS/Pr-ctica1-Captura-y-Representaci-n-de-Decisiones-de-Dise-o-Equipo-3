# Decisión de Diseño ADD-0004: Identificación del usuario.
* Status:proposed 
* Deciders: Antonio Agudo y Marcos Robles
* Date: 2020/11/24
## Context and Problem Statement
* Dado que de se debe almacenar un registro de los clientes y que estos deben hacer login para acceder a los diferentes microservicios, se necesita dar esta posibilidad al sistema mediante un logger que contará con una BBDD.
## Decision Drivers
* Los usuarios tienen datos propios como nombre o correo
* Todos esos datos deben almacenarse en una BBDD
* El cliente debe mandar la solicitud al servidor con los datos
## Considered Options
* (como expansión de la opción elegida)Usar un OTP (one time password) 
* (como expansión de la opción elegida)Usar verificación en 2 pasos
## Decision Outcome
* Chosen option:  un logger con una BBDD diseñado como microservicio independiente, ya que consideramos que es una base extensible a la que se le puede añadir otras mejoras de seguridad como OTP o verificación en 2 pasos. A nivel funcional recibirá los datos y devolverá una cookie que se usará para la identidad en el resto de microservicios.
 
### Positive Consequences
* Rápido tiempo de acceso
* Funcionamiento básico
* Ampliable
### Negative Consequences
* Problemas de seguridad a menos que se añada encriptación adicional
* La libre elección de contraseña del usuario puede suponer un problema de seguridad si no se tramita bien.
## Pros and Cons of the Options
## Usar un OTP (one time password) 
https://www.evidian.com/pdf/wp-strongauth-es.pdf

* Bueno, ya que añade otra capa de seguridad
* Malo, ya que si el usuario accede mucho puede resultar molesto
 
## Usar verificación en 2 pasos
Por ejemplo, usar el sistema de verificación de google en 2 pasos

* Bueno, ya que añade otra capa de seguridad
* Malo, ya que si el usuario accede mucho puede resultar molesto
* Malo, ya que el usuario puede perder el acceso a a la cuenta si pierde el dispositivo
* Malo, ya que puede resultar tedioso para el usuario hacer la verificación.





## Links <!-- optional -->

* [Definidido por RF0003](https://github.com/Grupo3-DAS/Pr-ctica1-Captura-y-Representaci-n-de-Decisiones-de-Dise-o-Equipo-3/blob/main/DAS-P1-Alba_Sevillano_Portilla-TAREA1.pdf) <!-- example: Refined by [ADR-0005](0005-example.md) -->
