# io-trilha-java-Bootcamp-Usando-Orienta-Objetos-em-Java
Desafio de código ofertado pela DIO- Abstraindo um Bootcamp Usando Orientação a Objetos em Java


## Diagrama UML (Mermaid)
```mermaid
classDiagram
    class Bootcamp {
        -nome:String
        -descricao:String
        -dataInitial:LocalDate
        -dataFinal:LocalDate
        -devsInscritos:Set
        -conteudos:Set
    }

    class Conteudo {
        #XP_PADRAO:double
        -titulo:String
        -descricao:String
        +calcularXP()void
    }

    class Curso {
        -cargaHoraria:int
        +calcularXP()void
        +toString()String
    }

    class Dev {
        -nome:String
        -conteudosInscritos:Set
        -conteudosConcluidos:Set
        +inscreverBootcamp(Bootcamp bootcamp)
        +progredir()void
        +calcularXP()void
    }

    class Mentoria {
        -data:LocalDate
        +calcularXP()void
        +toString()String
    }

    Bootcamp --> Conteudo
    Curso --> Conteudo
    Mentoria --> Conteudo
    Dev --> Bootcamp
    Dev -- Conteudo
```

## Referencia
[https://github.com/cami-la/desafio-poo-dio](Github do desafio)
[https://mermaid.js.org/intro/](Mermaid Docs)
