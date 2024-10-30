# Projeto de Autenticação com Spring Boot, Spring Security e JWT

Este projeto é uma API desenvolvida em Spring Boot que implementa autenticação e autorização de usuários utilizando Spring Security e JSON Web Tokens (JWT). O sistema permite a criação de usuários no banco de dados e efetua login aplicando JWT para autenticação e autorização.

## Tecnologias Utilizadas

- **Spring Boot**: Framework para desenvolvimento de aplicações Java.
- **Spring Security**: Framework que fornece segurança a aplicações.
- **JPA (Java Persistence API)**: API para interação com bancos de dados.
- **MySQL**: Banco de dados relacional utilizado para armazenar usuários.
- **JWT (JSON Web Tokens)**: Padrão aberto (RFC 7519) que define um método compacto e autocontido para transmitir informações entre partes de forma segura como um objeto JSON.

## Funcionalidades

- Registro de novos usuários
- Login de usuários com geração de token JWT
- Proteção de rotas com autorização baseada em roles
- Armazenamento seguro de senhas utilizando BCrypt

## Pré-requisitos

- Java 11 ou superior
- Maven
- MySQL

## Configuração do Banco de Dados

1. Crie um banco de dados no MySQL.
2. Configure as credenciais do banco de dados no arquivo `application.properties`:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/seu_banco_de_dados
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
