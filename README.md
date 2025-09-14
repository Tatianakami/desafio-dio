🚀 DIO - Trilha .NET | Nuvem com Microsoft Azure

Este projeto foi desenvolvido como parte do desafio da Digital Innovation One (DIO) no módulo de .NET com Microsoft Azure.

📌 Desafio de Projeto

Construir um sistema de RH em .NET, capaz de:

Cadastrar funcionários de uma empresa;

Implementar um CRUD completo (criar, ler, atualizar e deletar funcionários);

Registrar logs de alterações em funcionários, armazenados no Azure Table Storage.

A aplicação foi implantada no Microsoft Azure, utilizando:

App Service → para hospedar a API;

SQL Database → para o armazenamento relacional dos funcionários;

Azure Table Storage → para armazenar os logs de alterações.

🛠 Tecnologias Utilizadas

.NET 6 / C#

ASP.NET Core Web API

Entity Framework Core (com Migrations)

Swagger (documentação da API)

Azure App Service

Azure SQL Database

Azure Storage Account (Table Storage)

📂 Estrutura das Classes

📌 Classe Funcionario (dados principais)
📌 Classe FuncionarioLog (herda de Funcionario e registra alterações)

🔗 Endpoints Disponíveis
Método	Endpoint	Parâmetro	Body
GET	/Funcionario/{id}	id	N/A
POST	/Funcionario	N/A	Schema Funcionario
PUT	/Funcionario/{id}	id	Schema Funcionario
DELETE	/Funcionario/{id}	id	N/A
Exemplo de JSON (Funcionario)
{
  "nome": "Maria Souza",
  "endereco": "Rua das Flores, 123",
  "ramal": "1010",
  "emailProfissional": "maria.souza@empresa.com",
  "departamento": "TI",
  "salario": 5000,
  "dataAdmissao": "2025-01-10T08:00:00Z"
}

☁️ Arquitetura no Azure

O ambiente foi construído da seguinte forma:

App Service → Hospeda a API .NET

SQL Database → Armazena dados dos funcionários

Table Storage → Mantém os logs de alterações

✅ Resultado Final

O projeto foi concluído com sucesso:

CRUD funcional;

Logs persistidos corretamente;

Publicação no Azure validada.

📎 Acesse o código completo no repositório:
👉 GitHub - trilha-net-azure-desafio

**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body               |
|--------|-------------------------|-----------|--------------------|
| GET    | /Funcionario/{id}       | id        | N/A                |
| PUT    | /Funcionario/{id}       | id        | Schema Funcionario |
| DELETE | /Funcionario/{id}       | id        | N/A                |
| POST   | /Funcionario            | N/A       | Schema Funcionario |

Esse é o schema (model) de Funcionario, utilizado para passar para os métodos que exigirem:

```json
{
  "nome": "Nome funcionario",
  "endereco": "Rua 1234",
  "ramal": "1234",
  "emailProfissional": "email@email.com",
  "departamento": "TI",
  "salario": 1000,
  "dataAdmissao": "2022-06-23T02:58:36.345Z"
}
```





## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima, incluindo a sua publicação na nuvem.
