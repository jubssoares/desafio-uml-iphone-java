# Modelando o iPhone com UML: Funções de Músicas, Chamadas e Internet

<img align="right" height="200" style="border-radius:50px;" src="https://hermes.dio.me/tracks/a039b34c-7aa8-4a3d-b765-07c8c837f67a.png">

### Repositório criado para o desafio do bootcamp Santander 2024 - Backend com Java

<p align="justify">
    <br>
    O objetivo do desafio proposto é modelar e diagramar a representação UML do componente iPhone, abrangendo suas funcionalidades como Reprodutor Musical, Aparelho Telefônico e Navegador na Internet.
    <br>
</p>

<h4>Contexto</h4>

<p align="justify">
    Com base no vídeo de lançamento do iPhone de 2007 <a href="https://www.youtube.com/watch?v=9ou608QQRq8">(Link)</a>, elaborei a diagramação das classes e interfaces utilizando mermaid. Em seguida, implementei as classes e interfaces no formato de arquivos .java.
</p>

#### Funcionalidades a Modelar
1. **Reprodutor Musical**
   - Métodos: `tocar()`, `pausar()`, `selecionarMusica(String musica)`
2. **Aparelho Telefônico**
   - Métodos: `ligar(String numero)`, `atender()`, `iniciarCorreioVoz()`
3. **Navegador na Internet**
   - Métodos: `exibirPagina(String url)`, `adicionarNovaAba()`, `atualizarPagina()`

### Objetivo
1. Criar um diagrama UML que represente as funcionalidades descritas acima.
2. Implementar as classes e interfaces correspondentes em Java.


### Diagrama UML para o desafio proposto (Mermaid)

```mermaid
classDiagram
    class ReprodutorMusical {
        +void tocar()
        +void pausar()
        +void selecionarMusica(String musica)
    }

    class AparelhoTelefonico {
        +void ligar(String numero)
        +void atender()
        +void iniciarCorreioVoz()
    }

    class NavegadorInternet {
        +void exibirPagina(String url)
        +void adicionarNovaAba()
        +void atualizarPagina()
    }

    class iPhone {
        private String modelo
        private armazenamento
        private int capacidadeBateria
    }

    iPhone --> ReprodutorMusical
    iPhone --> AparelhoTelefonico
    iPhone --> NavegadorInternet
```