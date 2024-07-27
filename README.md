# io-trilha-java-Bootcamp-Usando-Orienta-Objetos-em-Java
Desafio de código ofertado pela DIO- Abstraindo um Bootcamp Usando Orientação a Objetos em Java


## Diagrama UML (Mermaid)
```mermaid
classDiagram
    class Bootcamp {
        -musicaAtual:Musica
        -musicas:List<Musica>
        +tocar()
        +pausar()
        +selecionarMusica(String musica)
    }

    class Conteudo {
        +ligar(String numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class Curso {
        -linkAtual:URL
        -linksAbertos:List<URL>
        +exibirPagina(String url)
        +adicionarNovaAba(URL url)
        +atualizarPagina()
    }

    class Dev {
        #reprodutor:ReprodutorMusical
        #telefone:AparelhoTelefonico
        #navegador:NavegadorInternet
    }

    class Mentoria {
        -titulo:String
        -autor:String
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
    Musica --> ReprodutorMusical
    URL --> NavegadorInternet
```

## Referencia
[https://github.com/cami-la/desafio-poo-dio](Github do desafio)
