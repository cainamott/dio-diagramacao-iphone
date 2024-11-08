@startuml
class Iphone

interface NavegadorNaInternet {
    + exibirPagina(String url)
    + adicionarNovaAba()
    + atualizarPagina()
}

interface ReprodutorMusical {
    + tocar()
    + pausar()
    + selecionarMusica(String musica)
}

interface AparelhoTelefonico {
    + ligar(String numero)
    + atender()
    + iniciarCorreioDeVoz()
}

Iphone ..|> NavegadorNaInternet
Iphone ..|> ReprodutorMusical
Iphone ..|> AparelhoTelefonico

@enduml