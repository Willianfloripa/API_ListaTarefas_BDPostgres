# ToDo List API

Uma API desenvolvida com **Spring Boot** para gerenciar tarefas (Lista de Tarefas), utilizando um banco de dados relacional **PostgreSQL**. O projeto foi projetado para permitir futuras integrações com frontend.

---

## 📋 Funcionalidades

- **Criar Tarefa**: Adiciona uma nova tarefa ao banco de dados.
- **Listar Tarefas**: Retorna todas as tarefas cadastradas.
- **Buscar Tarefa por ID**: Recupera uma tarefa específica pelo ID.
- **Atualizar Tarefa**: Altera os dados de uma tarefa existente.
- **Excluir Tarefa**: Remove uma tarefa pelo ID.

---

## 🛠️ Tecnologias Utilizadas

- **Java 21**
- **Spring Boot**:
  - Spring Web
  - Spring Data JPA
  - Spring Boot DevTools
- **PostgreSQL**
- **Lombok**
- **Maven**

---

## 🚀 Como Executar o Projeto

### Pré-requisitos

- [Java 21+](https://www.oracle.com/java/technologies/javase-jdk21-downloads.html)
- [Maven](https://maven.apache.org/)
- [PostgreSQL](https://www.postgresql.org/download/)
- [Postman](https://www.postman.com/) ou similar para testar a API

### Passo a Passo

1. **Clone o repositório**:
  No terminal execute:
   git clone https://github.com/Willianfloripa/ToDoList_API.git

   cd Lista_de_Tarefas_API

3. **Configure o banco de dados**:

  Crie um banco de dados PostgreSQL chamado todolist_db.
  No arquivo src/main/resources/application.properties, configure as credenciais do seu banco de dados:
  
  spring.datasource.url=jdbc:postgresql://localhost:5432/postgres
  spring.datasource.username=postgres
  spring.datasource.password=1234567
  
  spring.jpa.hibernate.ddl-auto=update
  spring.jpa.show-sql=true
  spring.jpa.properties.hibernate.format_sql=true
  spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect


3. **Compile e execute o projeto**:
  mvn spring-boot:run


4. **Teste os endpoints**:
  Utilize ferramentas como Postman ou Insomnia para interagir com a API.
Exemplo:
{
  "title": "Exemplo de Tarefa",
  "concluid": false
}

### 🧩 Estrutura do Projeto

 ![image](https://github.com/user-attachments/assets/34e235a5-1ecb-4cfb-aa36-2ab3f84bd373)


### 📝 Melhorias Futuras

  - Implementar autenticação e autorização (Spring Security).
  - Conectar um frontend (Angular).
  - Adicionar testes unitários e de integração.

### ✨ Autor
William Tonel de Melo

