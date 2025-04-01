# Criando API REST

Java RESTful API

## Diagrama de Classe

``` mermaid
classDiagram
    class Usuario {
        +String nome
        +Conta conta
        +Operacoes[] operacoes
        +Cartao cartao
        
    }

    class Conta {
        +String numero
        +String agencia
        +Float saldo
        +Float limite
    }

    class Operacoes {
        +String icone
        +String descricao
    }

    class Cartao {
        +String numero
        +Float limite
    }
    Usuario "1"*--"1" Conta 
    Usuario  "1"*--"n" Operacoes
    Usuario "1" *--"1" Cartao 
```
