# Criando API REST

Java RESTful API

## Diagrama de Classe

``` mermaid
classDiagram
    class ListaDeTarefas {
        +String nome
        +Tarefa[] tarefa
    }

    class Tarefa {
        +String nome
        +String descricao
        +String conclusao
    }
ListaDeTarefas "1" --> "n" Tarefa : contém
```
