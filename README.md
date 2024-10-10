# Mediotec Gerenciamento Escolar web

Este projeto consiste em um sistema escolar com um front-end em React e um back-end em Java com Spring Boot.

## Estrutura do Repositório

- **Front-End:** Repositório do front-end
- **Back-End:** Repositório do back-end

## Front-End

[Deploy do Front-End](https://mediotec.netlify.app)

### Tecnologias Usadas no Front-End

- React
- Tailwind CSS
- Vite

### Instalação do Front-End

1. Clone o repositório:
    ```bash
    git clone https://github.com/usuario/front-end-repo.git
    ```

2. Navegue até a pasta do projeto:
    ```bash
    cd front-end-repo
    ```

3. Instale as dependências:
    ```bash
    npm install
    ```

### Como Rodar o Front-End

1. Execute o comando:
    ```bash
    npm run dev
    ```

---

## Back-End

O back-end foi desenvolvido em Java com Spring Boot e está rodando no [Render](https://render.com) com um banco de dados PostgreSQL.

### [Deploy do Back-End](https://mediotec-backend.onrender.com)

### Tecnologias Usadas no Back-End

- Java 17+
- Spring Boot
- Maven
- PostgreSQL

### Configurações de Conexão com o Banco de Dados

O projeto está configurado para usar o PostgreSQL. Aqui estão as configurações de conexão padrão:

```properties
# Configurações de conexão com o banco de dados PostgreSQL
spring.datasource.url=jdbc:postgresql://${DB_HOST}:${DB_PORT}/${DB_NAME}
spring.datasource.username=${DB_USER}
spring.datasource.password=${DB_PASSWORD}
spring.datasource.driver-class-name=org.postgresql.Driver

# Configurações do JPA/Hibernate
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

# Dialeto do PostgreSQL para o Hibernate
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.PostgreSQLDialect

# Configurações adicionais (opcionais)
spring.jpa.properties.hibernate.format_sql=true
spring.jpa.properties.hibernate.use_sql_comments=true
