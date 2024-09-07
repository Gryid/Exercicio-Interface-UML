
# Exercicio UML Java

- Exercico de criação de UML para representar a implementação de interfaces.
- Exemplo de implementação de uma UML com base nas funcionalidades (Aparelho telefonico, Reprodutor Musical, Navegador) do Iphone.

```mermaid
classDiagram
    
    class Iphone {
        -int numeroSerie
    } 
    
    class navegadorInternet {
      +exibirPagina()
      +adicionarNovaAba()
      +atualizarPagina()
    }
    class aparelhoTelefonico {
      +atender()
      +ligar()
      +iniciarCorreioVoz()
    }
    class reprodutorMusical {
      +tocar()
      +pausar()
      +selecionarMusica()
    }

    Iphone ..|> navegadorInternet
    Iphone ..|> aparelhoTelefonico
    Iphone ..|> reprodutorMusical
