# API RESTFul com Java e Spring Boot

## Descrição

API RESTFul com Java e Spring Boot

## Tecnologias

- Java 22
- Spring Boot 3.3.2
- Gradle

## Arquitetura

- Controller
- Service
- Repository
- Model
- DTO

> [!INFO]  
> **DTO** (Data Transfer Object) é um padrão de projeto cujo objetivo é transferir dados entre subsistemas de um software.  
> No nosso caso, utilizaremos para transportar dados entre diferentes camadas da aplicação sem expor as entidades do banco de dados diretamente.

## Infraestrutura

- Banco de Dados: PostgreSQL
- Hospedagem: Railway
- ~~CI/CD: GitHub Actions~~

> [!INFO]
> **Procfile**: arquivo que informa ao Railway como iniciar a aplicação.

> [!WARNING]
> Caso o Railway falhe durante o deploy por conta da versão atual do Gradle ser muito recente, acesse o arquivo `gradle-wrapper.properties` presente em `gradle/wrapper` e altere a versão do Gradle para uma mais antiga.  
> 
> Exemplo:
> ```properties
> distributionUrl=https\://services.gradle.org/distributions/gradle-7.6.1-bin.zip
> ```