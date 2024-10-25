# CRUD com Spring Boot

Este projeto é uma aplicação simples de CRUD (Create, Read, Update, Delete) para gerenciamento de produtos, desenvolvida em **Java** com **Spring Boot**. A interface front-end é implementada utilizando **Thymeleaf**, e a aplicação se conecta a um banco de dados MySQL para persistir as informações dos produtos.

## Funcionalidades

- Listar produtos
- Criar novos produtos
- Editar produtos existentes
- Deletar produtos

## Tecnologias Utilizadas

- **Java**: Linguagem de programação principal
- **Spring Boot**: Framework para criar aplicações Java simplificadas
- **Thymeleaf**: Motor de templates para renderizar HTML no servidor
- **MySQL**: Banco de dados para armazenar informações dos produtos
- **JPA/Hibernate**: Mapeamento objeto-relacional (ORM) para interação com o banco de dados

## Instalação e Execução

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
    ```
2. Navegue até a pasta do projeto:
   ```bash
   cd nome-do-repositorio
   ```
3. Configure o banco de dados MySQL com as seguintes propriedades:
```bash
    spring.datasource.url=jdbc:mysql://localhost:3306/crud_db
    spring.datasource.username=seu-usuario
    spring.datasource.password=sua-senha
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect
```
4. Execute o projeto usando o Maven:
   ```bash
   mvn spring-boot:run
   ```
5. Acesse a aplicação no navegador:
   ```
   http://localhost:8080/products
   ```
## Estrutura do Projeto
- controller/: Contém os controladores Spring que lidam com as requisições HTTP.
- model/: Contém as classes modelo que representam as entidades no banco de dados.
- repository/: Contém as interfaces de repositório para interagir com o banco de dados usando JPA.
- templates/: Contém os templates Thymeleaf utilizados para renderizar as páginas HTML.
## Melhorias Futuras
- Adicionar validação de dados nos formulários.
- Implementar paginação na listagem de produtos.
- Testes unitários para os serviços e controladores.