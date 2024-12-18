# Servidor de Configuración

Este proyecto es un servidor de configuración basado en Spring Boot que proporciona configuraciones centralizadas para microservicios. El servidor de configuración se conecta a un repositorio Git para obtener las configuraciones y las expone a los microservicios que se registran en el servidor Eureka y se comunican a través de un API Gateway.

## Características

- **Spring Boot**: Utiliza Spring Boot para facilitar la configuración y el despliegue.
- **Spring Cloud Config Server**: Proporciona configuraciones centralizadas para microservicios.
- **Git**: Las configuraciones se almacenan en un repositorio Git.
- **Eureka Server**: Los microservicios se registran en un servidor Eureka.
- **API Gateway**: Los microservicios se comunican a través de un API Gateway.

## Requisitos

- Java 11 o superior
- Maven 3.6.0 o superior

## Configuración

El archivo `application.properties` contiene la configuración del servidor de configuración:

```ini
# Configuración del servidor de configuración
spring.application.name=ServidorConfiguracion
server.port=8888
spring.cloud.config.server.git.uri=https://github.com/WakandaForeverPC/ConfiguracionesMicroservicios.git
spring.cloud.config.server.git.clone-on-start=true
