# Santander Bootcamp Fullstack 2023 - REST API em Java + Tech Stack
Bem-vindo ao repositório da RESTful API feita para a entrega do último projeto do Bootcamp Fullstack da Santander em 2023, hospedado pela DIO. Esta API foi construída em Java 17 com o framework Spring Boot 3.

## Autores
- [DIO (pela base)](https://github.com/digitalinnovationone)
- [Emanuel Messias](https://github.com/messiasof)

## Sobre o Projeto
Este é um projeto simples que serve como uma API para a entrega do último projeto do Santander Bootcamp Fullstack 2023, da plataforma Digital Innovation One (DIO). Esta API é parte integrante de uma aplicação mais ampla, permitindo a interação com o sistema e fornecendo funcionalidades essenciais.

## Tecnologias Principais
- **Java 17**: Utilizamos a versão LTS mais recente do Java para aproveitar as inovações mais recentes desta linguagem amplamente utilizada.
- **Spring Boot 3**: Esta é a versão mais recente do Spring Boot, que oferece autoconfiguração poderosa, aumentando a produtividade do desenvolvedor.
- **Spring Data JPA**: Simplificamos o acesso aos dados com o Spring Data JPA, facilitando a integração com bancos de dados SQL.
- **OpenAPI (Swagger)**: Criamos uma documentação de API eficaz e fácil de entender usando a OpenAPI (Swagger), alinhada com a alta produtividade do Spring Boot.
- **Railway**: Facilita o deploy e monitoramento de soluções na nuvem, oferecendo diversos bancos de dados como serviço e pipelines de CI/CD. Esta API estará disponível no Railway por um período limitado, mas é um projeto de código aberto. Sinta-se à vontade para cloná-lo, modificá-lo e executá-lo localmente ou onde desejar.

## Diagrama de Classes (Domínio da API)
O diagrama abaixo representa as principais classes que compõem o domínio desta API conforme o fork original:

```mermaid
classDiagram
  class User {
    -String name
    -Account account
    -Feature[] features
    -Card card
    -News[] news
  }

  class Account {
    -String number
    -String agency
    -Number balance
    -Number limit
  }

  class Feature {
    -String icon
    -String description
  }

  class Card {
    -String number
    -Number limit
  }

  class News {
    -String icon
    -String description
  }

  User "1" *-- "1" Account
  User "1" *-- "N" Feature
  User "1" *-- "1" Card
  User "1" *-- "N" News
  ```

Sinta-se livre pra modificar como quiser
