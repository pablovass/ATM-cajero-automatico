# Proyecto Cajero Automático (ATM) - Prototipo

## Descripción del Proyecto

Este repositorio contiene el código fuente de un prototipo de cajero automático (ATM) implementado mediante dos microservicios en Java 17 con Spring Boot. Los microservicios se encargan de la gestión de clientes y la gestión de transacciones monetarias. Además, se utiliza MongoDB y MySQL como bases de datos, Kafka para la gestión de eventos y Docker para la contenerización de la aplicación.

La interfaz de usuario está desarrollada con React, proporcionando una experiencia amigable e intuitiva para los usuarios finales.

## Tecnologías Utilizadas

- **Microservicios**: Desarrollados en Java 17 con Spring Boot.
  - **Gestión de Clientes**: Microservicio encargado de la gestión de clientes.
  - **Gestión Monetaria**: Microservicio responsable de las transacciones monetarias.

- **Bases de Datos**:
  - **MongoDB**: Utilizado para almacenar información relacionada con clientes.
  - **MySQL**: Utilizado para almacenar datos transaccionales y financieros.

- **Event-Driven Architecture**:
  - **Kafka**: Se emplea como sistema de mensajería para implementar una arquitectura basada en eventos.

- **Contenerización**:
  - **Docker**: La aplicación está contenerizada para facilitar la implementación y la escalabilidad.

- **Interfaz de Usuario**:
  - **React**: La interfaz de usuario se desarrolla utilizando React para una experiencia de usuario moderna y receptiva.

## Configuración y Despliegue

1. **Configuración de Microservicios**:
   - Asegúrese de tener Java 17 instalado.
   - Configure las propiedades de conexión a las bases de datos en los archivos de configuración de cada microservicio.

2. **Configuración de Bases de Datos**:
   - Instale y configure MongoDB y MySQL según las necesidades del proyecto.

3. **Configuración de Kafka**:
   - Asegúrese de tener un clúster de Kafka disponible.
   - Configure las propiedades de conexión en los microservicios que interactúan con Kafka.

4. **Contenerización con Docker**:
   - Utilice los archivos de configuración proporcionados para construir imágenes Docker de los microservicios y la interfaz de usuario.

5. **Despliegue**:
   - Despliegue los contenedores Docker en el entorno deseado.

## Estructura del Proyecto

```plaintext
/proyecto-cajero-automatico
|-- /gestion-clientes-service
|   |-- ...
|
|-- /gestion-monetaria-service
|   |-- ...
|
|-- /react-ui
|   |-- ...
|
|-- docker-compose.yml
|-- README.md
|-- ...

```
### Contribución
¡Las contribuciones son bienvenidas! Si encuentra algún problema o tiene sugerencias, por favor, abra un problema en el repositorio. Si desea contribuir con código, realice una solicitud de extracción.

### Licencia
Este proyecto está bajo la Licencia MIT. ¡Siéntase libre de utilizar, modificar y distribuir según sus necesidades!



Puedes copiar y pegar este contenido en tu `README.md` y ajustarlo según tus necesidades. ¡Buena suerte con tu proyecto!
