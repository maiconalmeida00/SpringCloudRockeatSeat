# ☁️ Projeto Spring Cloud com Docker

Este projeto foi desenvolvido em **Java** utilizando o **Spring Cloud**, com o objetivo de demonstrar a construção de uma arquitetura baseada em **microsserviços**.  
A aplicação é totalmente containerizada com **Docker**, facilitando o deploy e a escalabilidade.

---

## 🚀 Tecnologias Utilizadas

- **Java 17+**
- **Spring Boot**
- **Spring Cloud (Eureka, Gateway, Config Server, etc.)**
- **Maven**
- **Docker e Docker Compose**
- **PostgreSQL / MySQL** (caso o projeto utilize banco de dados)
- **Lombok**

---

## ⚙️ Estrutura do Projeto

```plaintext
📦 spring-cloud-docker-project
 ┣ 📂 config-server        # Servidor de configuração centralizada
 ┣ 📂 eureka-server        # Service Discovery (Eureka)
 ┣ 📂 api-gateway          # Roteamento e autenticação das requisições
 ┣ 📂 service-user         # Microsserviço responsável pelos usuários
 ┣ 📂 service-product      # Microsserviço responsável pelos produtos
 ┣ 📜 docker-compose.yml   # Orquestração dos containers
 ┣ 📜 README.md            # Documentação do projeto
 ┗ 📜 pom.xml              # Configuração Maven principal
