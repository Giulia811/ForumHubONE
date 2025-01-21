# 🚀 Forum API Challenge

Este projeto consiste na criação de uma API Restful para um fórum, desenvolvida com **Spring Boot** e **MySQL**. A aplicação oferece funcionalidades para gerenciamento de usuários, tópicos e respostas, implementando boas práticas de design e persistência de dados.

## 🎯 Objetivos do Projeto

- Desenvolver uma API Restful para gerenciamento de usuários, tópicos e respostas.
- Implementar persistência de dados utilizando o banco de dados MySQL.
- Seguir as boas práticas de design de APIs.
- Utilizar Spring Boot como framework principal para o desenvolvimento.

## 🛠️ Tecnologias Utilizadas

- **Java 17**
- **Spring Boot 3.x**
- **JPA/Hibernate**
- **Spring Security**
- **Spring Doc**
- **Bean Validation**
- **Lombok**
- **Flyway**
- **Auth0** (para tokens JWT)
- **IntelliJ**
- **Git**
- **MySQL 8.x**

## 📋 Funcionalidades

A API fornece endpoints para:

### 👤 Usuários
- **Criar um usuário**
- **Listar todos os usuários**
- **Buscar um usuário por ID**
- **Atualizar um usuário**
- **Excluir um usuário**

### 📂 Tópicos
- **Criar um tópico**
- **Listar todos os tópicos**
- **Buscar um tópico por ID**
- **Atualizar um tópico**
- **Excluir um tópico**

### 💬 Respostas
- **Adicionar uma resposta a um tópico**
- **Listar todas as respostas de um tópico**
- **Atualizar uma resposta**
- **Excluir uma resposta**

## 🗂️ Estrutura do Projeto

O projeto segue a arquitetura MVC (Model-View-Controller) e está organizado da seguinte forma:

```
📂 src
├── 📁 main
│   ├── 📁 java/br/com/forumhub
│   │   ├── 📂 controller
│   │   ├── 📂 domain
│   │   ├── 📂 infra
│   │   ├── 📂 util
│   │   └── 📄 ForumhubApplication.java
│   ├── 📂 resources
│       ├── 📂 db/migration
│       └── 📄 application.properties
├── 📂 test/java/br/com/forumhub
│   └── 📄 ForumhubApplicationTests.java
├── 📄 README.md
├── 📄 mvnw
├── 📄 mvnw.cmd
└── 📄 pom.xml
```

## ⚙️ Configuração do Ambiente

### Pré-requisitos

1. **Java 17** ou superior.
2. **MySQL**.
3. **Maven** instalado.

### Passos para Configuração

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/forum-api.git
   ```

2. Configure o banco de dados no arquivo `application.properties`:
   ```properties
   spring.application.name=forumhub
   spring.datasource.url=jdbc:mysql://${DB_HOST}/forum_hub
   spring.datasource.username=${DB_USER}
   spring.datasource.password=${DB_PASSWORD}
   #server.error.include-stacktrace=never
   api.security.token.secret=${JWT_SECRET:12345678}
   #spring.jpa.hibernate.ddl-auto=update
   ```

3. Execute o projeto:
   ```bash
   mvn spring-boot:run
   ```

4. Acesse a API em `http://localhost:8080`.

## 🚀 Próximos Passos

- Implementar autenticação e autorização com **Spring Security**.
- Criar testes unitários e de integração.
- Adicionar paginação e ordenação nos endpoints de listagem.
- Melhorar a documentação utilizando **Swagger/OpenAPI**.

## 🤝 Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.

