# decola-tec-2025
Java RESTful API criada para o decola tec 2025

## Diagrama de Classes

```mermaid
classDiagram
    class Inscricao {
        +string nome
    }

    class Bootcamp {
        +string etapa
        +string descricao
        +string status
    }

    class Entrevista {
        +string etapa
        +string descricao
        +string status
    }

    class TesteLogica {
        +string etapa
        +string descricao
        +string status
    }

    class TesteLinguaInglesa {
        +string etapa
        +string descricao
        +string status
    }

    class EntrevistaRH {
        +string etapa
        +string descricao
        +string status
    }

    class EntrevistaTecnica {
        +string etapa
        +string descricao
        +string status
    }

    class ResultadoProcessoSeletivo {
        +string etapa
        +string descricao
        +string status
    }

    class AprovadoEcolhimento {
        +string etapa
        +string descricao
        +string status
    }

    Inscricao <|-- Bootcamp : "inicia"
    Inscricao <|-- Entrevista : "inicia"
    Inscricao <|-- TesteLogica : "inicia"
    Inscricao <|-- TesteLinguaInglesa : "inicia"
    Inscricao <|-- EntrevistaRH : "inicia"
    Inscricao <|-- EntrevistaTecnica : "inicia"
    Inscricao <|-- ResultadoProcessoSeletivo : "inicia"
    ResultadoProcessoSeletivo <|-- AprovadoEcolhimento : "aprovação"
