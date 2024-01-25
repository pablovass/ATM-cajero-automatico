# API-ATM - Spring Boot 3 (Java 17) - Proyecto de Cajero Automático

## Descripción del Proyecto

Bienvenido al repositorio de API-ATM, un proyecto desarrollado en Spring Boot 3 con Java 17 y gestionado con Gradle. Este proyecto se centra en la implementación de la funcionalidad principal de un cajero automático (ATM). Aunque la elección de la base de datos aún no está determinada, la aplicación está diseñada para ser contenerizada con Docker para facilitar el despliegue y la gestión del entorno.

## Tecnologías Utilizadas

- **Java 17**: Utilizado como lenguaje de programación principal.
- **Spring Boot 3**: Marco de desarrollo para aplicaciones Java basado en Spring.
- **Gradle**: Herramienta de construcción y gestión de dependencias.
- **Docker**: Contenerización para facilitar el despliegue y la administración del entorno.

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
   docker build -t api-atm:latest .
   ```

5. **Despliegue**:
    - Despliegue el contenedor Docker en el entorno deseado.

## Estructura del Proyecto

```plaintext
/api-atm
|-- /src
|   |-- /main
|   |   |-- /java
|   |   |   |-- ...
|   |   |
|   |   |-- /resources
|   |   |   |-- application.properties
|   |   |   |-- ...
|   |
|   |-- /build.gradle
|-- README.md
|-- ...
```

## Contribución

¡Las contribuciones son bienvenidas! Si encuentra algún problema o tiene sugerencias, por favor, abra un problema en el repositorio. Si desea contribuir con código, realice una solicitud de extracción.

## Licencia

Este proyecto está bajo la Licencia [MIT](LICENSE). ¡Siéntase libre de utilizar, modificar y distribuir según sus necesidades!

---

¡Gracias por contribuir al desarrollo de API-ATM! Si tienes alguna pregunta o necesitas ayuda, no dudes en ponerte en contacto. ¡Éxito en tu desarrollo!