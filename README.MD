
# Exercicio UML Java

- Exercico de criação de UML para representar a implementação de interfaces.
- Exemplo de implementação de uma UML com base nas funcionalidades (Aparelho telefonico, Reprodutor Musical, Navegador) do Iphone.

```mermaid
classDiagram
    
    class Iphone {
        -int numeroSerie
    } 
    
    interface navegadorInternet {
      +exibirPagina()
      +adicionarNovaAba()
      +atualizarPagina()
    }
    interface aparelhoTelefonico {
      +atender()
      +ligar()
      +iniciarCorreioVoz()
    }
    interface reprodutorMusical {
      +tocar()
      +pausar()
      +selecionarMusica()
    }

    Iphone ..|> navegadorInternet
    Iphone ..|> aparelhoTelefonico
    Iphone ..|> reprodutorMusical
