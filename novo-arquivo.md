classDiagram
    class iPhone {
        +ReprodutorMusical reprodutor
        +AparelhoTelefonico telefone
        +NavegadorInternet navegador
    }

    class ReprodutorMusical {
        +tocar()
        +pausar()
        +selecionarMusica(string Musica)
    }

    class AparelhoTelefonico {
        +ligar(string Numero)
        +atender()
        +iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +exibirPagina(string url)
        +adicionarNovaAba()
        +atualizarPagina()
    }

    iPhone --> ReprodutorMusical : contem
    iPhone --> AparelhoTelefonico : contem
    iPhone --> NavegadorInternet : contem