# DIO - Trilha .NET - API e Entity Framework
www.dio.me

## Desafio de projeto
Para este desafio, você precisará usar seus conhecimentos adquiridos no módulo de API e Entity Framework, da trilha .NET da DIO.

## Contexto
Você precisa construir um sistema gerenciador de tarefas, onde você poderá cadastrar uma lista de tarefas que permitirá organizar melhor a sua rotina.

Essa lista de tarefas precisa ter um CRUD, ou seja, deverá permitir a você obter os registros, criar, salvar e deletar esses registros.

A sua aplicação deverá ser do tipo Web API ou MVC, fique a vontade para implementar a solução que achar mais adequado.

A sua classe principal, a classe de tarefa, deve ser a seguinte:

![Diagrama da classe Tarefa](diagrama.png)

Não se esqueça de gerar a sua migration para atualização no banco de dados.

## Métodos esperados
É esperado que você crie o seus métodos conforme a seguir:


**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**


| Verbo  | Endpoint                                                                 | Parâmetro         | Body          |
|--------|--------------------------------------------------------------------------|-------------------|---------------|
| GET    | [/Tarefa/{id}](Controllers/TarefaController.cs#L20)                      | id                | N/A           |
| PUT    | [/Tarefa/{id}](Controllers/TarefaController.cs#L98)                      | id                | Schema Tarefa |
| DELETE | [/Tarefa/{id}](Controllers/TarefaController.cs#L120)                     | id                | N/A           |
| GET    | [/Tarefa/ObterTodos](Controllers/TarefaController.cs#L31)                | N/A               | N/A           |
| GET    | [/Tarefa/ObterPorTitulo](Controllers/TarefaController.cs#L42)            | titulo            | N/A           |
| GET    | [/Tarefa/ObterPorData](Controllers/TarefaController.cs#L53)              | data              | N/A           |
| GET    | [/Tarefa/ObterPorStatus](Controllers/TarefaController.cs#L64)            | status            | N/A           |
| GET    | [/Tarefa/ObterPorTituloOuDescricao](Controllers/TarefaController.cs#L75) | titulo\|descricao | N/A           |
| POST   | [/Tarefa](Controllers/TarefaController.cs#L86)                           | N/A               | Schema Tarefa |

Esse é o schema (model) de Tarefa, utilizado para passar para os métodos que exigirem

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```


## Solução
O código está pela metade, e você deverá dar continuidade obedecendo as regras descritas acima, para que no final, tenhamos um programa funcional. Procure pela palavra comentada "TODO" no código, em seguida, implemente conforme as regras acima.

**Resolvido!**
