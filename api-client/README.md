# API-Client - Spring Boot 3 (Java 17) - Gestión de Clientes para Cajero Automático

## Descripción del Proyecto

¡Bienvenido al repositorio de API-Client! Este proyecto, desarrollado en Spring Boot 3 con Java 17 y gestionado con Gradle, se centra en la gestión de clientes para un cajero automático (ATM). La aplicación seguirá los principios de SOLID y estará diseñada con una arquitectura hexagonal para garantizar la escalabilidad y la modularidad del sistema. Además, se prevé la contenerización con Docker para facilitar el despliegue y la administración del entorno.

## Tecnologías Utilizadas

- **Java 17**: Utilizado como lenguaje de programación principal.
- **Spring Boot 3**: Marco de desarrollo para aplicaciones Java basado en Spring.
- **Gradle**: Herramienta de construcción y gestión de dependencias.
- **Docker**: Contenerización para facilitar el despliegue y la administración del entorno.
- **SOLID**: Principios de diseño para escribir código mantenible y escalable.
- **Arquitectura Hexagonal**: Diseño modular y escalable para facilitar el desarrollo y la prueba.

## Configuración y Desarrollo

1. **Requisitos Previos**:
   - Asegúrese de tener Java 17 instalado en su sistema.
   - Instale Gradle para gestionar las dependencias y construir el proyecto.

2. **Configuración del Proyecto**:
   - Clone este repositorio en su máquina local.
   - Configure las propiedades del proyecto según sea necesario (por ejemplo, puertos, rutas).

3. **Desarrollo Local**:
   - Ejecute la aplicación localmente para el desarrollo y pruebas.
   ```bash
   gradle bootRun
   ```

4. **Contenerización con Docker**:
   - Utilice Docker para contenerizar la aplicación.
   ```bash
   docker build -t api-client:latest .
   ```

5. **Despliegue**:
   - Despliegue el contenedor Docker en el entorno deseado.

## Estructura del Proyecto

```plaintext
/api-client
|-- /src
|   |-- /main
|   |   |-- /java
|   |   |   |-- /com
|   |   |       |-- /yourcompany
|   |   |           |-- /atm
|   |   |               |-- /client
|   |   |                   |-- ...
|   |   |
|   |   |-- /resources
|   |   |   |-- application.properties
|   |   |   |-- ...
|   |
|   |-- /build.gradle
|-- README.md
|-- ...
```

## Principios SOLID

- **[S] Single Responsibility Principle (SRP)**: Cada clase debería tener una única razón para cambiar.
- **[O] Open/Closed Principle (OCP)**: La clase debe estar abierta para la extensión pero cerrada para la modificación.
- **[L] Liskov Substitution Principle (LSP)**: Las instancias de una clase derivada deberían poder reemplazar instancias de la clase base.
- **[I] Interface Segregation Principle (ISP)**: Un cliente no debería verse obligado a depender de interfaces que no utiliza.
- **[D] Dependency Inversion Principle (DIP)**: Las dependencias deben ser en torno a abstracciones, no a detalles.

## Arquitectura Hexagonal

La arquitectura hexagonal se implementará para garantizar la separación de las preocupaciones y facilitar la prueba de cada componente de la aplicación.

```plaintext
/api-client
|-- /src
|   |-- /main
|   |   |-- /java
|   |   |   |-- /com
|   |   |       |-- /yourcompany
|   |   |           |-- /atm
|   |   |               |-- /client
|   |   |                   |-- /domain
|   |   |                   |-- /ports
|   |   |                   |-- /adapters
|   |   |
|   |   |-- /resources
|   |   |   |-- application.properties
|   |   |   |-- ...
|   |
|   |-- /build.gradle
|-- README.md
|-- ...
```

- **Domain**: Contiene la lógica de negocio y las entidades de dominio.
- **Ports**: Define las interfaces que permiten a los adaptadores interactuar con el sistema.
- **Adapters**: Implementa las interfaces definidas en Ports y actúa como puente entre el sistema y los elementos externos.

## Contribución

¡Las contribuciones son bienvenidas! Si encuentra algún problema o tiene sugerencias, por favor, abra un problema en el repositorio. Si desea contribuir con código, realice una solicitud de extracción.

## Licencia

Este proyecto está bajo la Licencia [MIT](LICENSE). ¡Siéntase libre de utilizar, modificar y distribuir según sus necesidades!

---

¡Gracias por contribuir al desarrollo de API-Client! Si tienes alguna pregunta o necesitas ayuda, no dudes en ponerte en contacto. ¡Éxito en tu desarrollo!