# Discovery Server com Eureka  
## Introdução  Este projeto é um Discovery Server desenvolvido em Java utilizando o **Eureka** da Netflix.
Ele faz parte de um sistema de agendamento de quadras, permitindo que os microserviços se registrem e descubram uns aos outros de forma dinâmica.  
## Tecnologias Utilizadas  
- **Java**: Linguagem de programação principal.
- **Spring Boot**: Framework para facilitar a criação de aplicações Java.
- **Eureka Server**: Serviço de registro e descoberta de microserviços.


## Configuração do Projeto  
### Dependência:  
```xml
<dependency>
  <groupId>org.springframework.cloud</groupId>
  <artifactId>spring-cloud-starter-netflix-eureka-server</artifactId>
</dependency>
```
### Application.yml:  
```yml
spring:
  application:
    name: discovery-server

server:
  port: 8761

eureka:
  client:
    register-with-eureka: false
    fetch-registry: false
```
