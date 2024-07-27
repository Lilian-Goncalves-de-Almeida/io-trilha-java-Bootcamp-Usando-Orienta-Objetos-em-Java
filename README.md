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

    abstract Conteudo {
        #XP_PADRAO:double
        -titulo:String
        -descricao:String
        +calcularXP()
    }

    class Curso {
        -cargaHoraria:int
        +calcularXP()
        +toString()
    }

    class Dev {
        -nome:String
        -conteudosInscritos:Set
        -conteudosConcluidos:Set
        +inscreverBootcamp(Bootcamp bootcamp)
        +progredir():void
        +calcularXP()
    }

    class Mentoria {
        -data:LocalDate
        +calcularXP()
        +toString()
    }

    Bootcamp --> Conteudo
    Curso --> Conteudo
    Mentoria --> Conteudo
    Dev --> Bootcamp
    Dec -- Conteudo
```

## Referencia
[https://github.com/cami-la/desafio-poo-dio](Github do desafio)
