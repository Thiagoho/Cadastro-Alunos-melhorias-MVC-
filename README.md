## Desafio — Cadastro de Alunos (Spring Boot + MVC + DTO)

Este projeto é um desafio prático com foco em backend utilizando **Java com Spring Boot**. O objetivo é construir uma API RESTful para gerenciar um sistema simples de **cadastro de alunos**, seguindo o padrão **MVC** e aplicando conceitos de camadas (Controller, Service, Repository e DTO).

---
## Objetivo
- Criar uma API RESTful utilizando Spring Boot.
- Implementar boas práticas como uso de DTOs e separação de responsabilidades.
- Simular as operações básicas de CRUD (Create, Read, Update, Delete).

---

## Estrutura do Projeto
src/main/java/com/desafio/aluno/<br>
├── controller/ # Camada que lida com requisições HTTP (API)<br>
│ └── AlunoController.java<br>
├── dto/ # Objetos de transferência de dados (entrada/saída)<br>
│ └── AlunoDto.java<br>
├── model/ # Entidade JPA "Aluno"<br>
│ └── Aluno.java<br>
├── repository/ # Interface de acesso ao banco de dados<br>
│ └── AlunoRepository.java<br>
└── service/ # Regras de negócio<br>
└── AlunoService.java<br>
### Tecnologias Utilizadas
Java 17+
Spring Boot
Spring Data JPA
Banco de Dados H2 (pode ser trocado por MySQL/PostgreSQL)
Maven
Swagger (opcional)
### Como executar o projeto
Clone o repositório:
git clone https://github.com/seu-usuario/desafio-cadastro-alunos.git
### Navegue até o diretório:
cd desafio-cadastro-alunos
### Execute o projeto com:
./mvnw spring-boot:run
### Acesse o Swagger (se configurado):
http://localhost:8080/swagger-ui.html
<h4>Autor

Thiago Henrique de Oliveira Sales
Estudante de ADS, desenvolvendo habilidades em backend Java.</h4>
###  Endpoints da API

| Método | Endpoint         | Descrição                        |
|--------|------------------|----------------------------------|
| GET    | `/alunos`        | Listar todos os alunos           |
| GET    | `/alunos/{id}`   | Buscar aluno por ID              |
| POST   | `/alunos`        | Cadastrar novo aluno             |
| PUT    | `/alunos/{id}`   | Atualizar dados de um aluno      |
| DELETE | `/alunos/{id}`   | Deletar aluno por ID             |

---

### Exemplos de Requisições

###  POST `/alunos`

```json
{
  "nome": "Maria Oliveira",
  "email": "maria@email.com"
}
