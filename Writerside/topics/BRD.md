# BRD

> **Definição de BRD**
>
> Um Business Requirements Document (BRD) é um relatório detalhado que descreve tudo o que um novo projeto requer para obter sucesso. Este documento delineia os objetivos do projeto, o que é esperado ao longo do ciclo de vida do projeto e o que é necessário para o alcançar.
> {style="note"}

## Objetivo do projeto

O **%product%** é um sistema de avaliação colaborativa onde os utilizadores votam em "cartas" que representam as competências e o desempenho de profissionais ou estudantes.

O objetivo do projeto é simplificar a complexa tarefa de avaliação de competências através de um sistema de cartas gamificado. Em vez de avaliar uma pessoa diretamente, os utilizadores avaliam uma carta que abstrai as suas qualidades, tornando o processo mais objetivo e focado nas habilidades. A avaliação será feita por meio de atributos pré-definidos, como por exemplo:

-   Comunicação
-   Trabalho em Equipe
-   Proatividade
-   Colaboração

Os resultados da avaliação serão exibidos em cartas que representam o perfil avaliado, com os valores de seus atributos. Os utilizadores podem então montar equipas (decks) com as cartas para participar em torneios ou simular a força de um grupo, permitindo análises detalhadas sobre o desempenho individual e em equipa.

## Escopo do projeto

### Objetivo principal do projeto

Implementar um sistema web que permita a avaliação entre utilizadores em formato de cartas de baralho, promovendo uma análise de desempenho gamificada e colaborativa.

### Funcionalidades incluídas

-   **Cadastro e Login de Utilizadores**: Sistema padrão de autenticação para acesso à plataforma.
-   **Criação e Gestão de Cartas**: Utilizadores podem criar e gerir as suas próprias cartas, que representam o seu perfil profissional ou académico.
-   **Votação em Cartas**: Participar na avaliação de perfis votando nas cartas para valorar as suas competências.
-   **Fóruns de Discussão**: Cada carta terá um espaço de fórum dedicado para que os utilizadores possam discutir e aprofundar a análise sobre o perfil representado.
-   **Montagem de Decks**: Construir "decks" ou equipas combinando diferentes cartas para fins estratégicos.
-   **Torneios e Simulações**: Participar em torneios com os decks ou simular a eficácia de uma equipa para analisar a sinergia entre as cartas.
-   **Rankings**: Sistema de ranking para alunos, equipas e um ranking geral para incentivar a melhoria contínua.

### Regras que impactam o desenvolvimento

-   Cada utilizador só pode criar a sua própria carta (Em análise).
-   Uma carta só pode ser avaliada uma vez por utilizador para garantir a justiça na avaliação.
-   As avaliações são anônimas para promover a honestidade no feedback.
-   O rank é reiniciado a cada módulo (temporada) para dar a todos a oportunidade de melhorar.

### Sistemas envolvidos

-   Serviço de autenticação de utilizadores (User service Opaleiros).

### Usuários envolvidos

-   Alunos e profissionais da instituição que utilizarão o sistema.

### Restrições técnicas ou operacionais

-   O sistema deve ser uma aplicação web responsiva, compatível com navegadores modernos.
-   A plataforma será totalmente online.

### Premissas do projeto

-   Os votos serão reiniciados a cada módulo (temporada) para que todos tenham a chance de se redimir e melhorar no rank.

### O que está fora do escopo (out of scope)

-   Qualquer funcionalidade não listada explicitamente no escopo do projeto.

## Requerimentos de Negócios

> MVP 1.0

| Requisito de Negócio | Prioridade | Nível Crítico |
|---|---|---|
| Cadastro e Login de Utilizadores | 1 | Crítico |
| Criação e Gestão de Cartas | 1 | Crítico |
| Votação em Cartas | 1 | Crítico |
| Rankings (Alunos, Equipas, Geral) | 1 | Crítico |
| Montagem de Decks e Simulações | 2 | Médio |
| Fóruns de Discussão | 2 | Médio |
| Reset do rank a cada fim de módulo | 2 | Médio |
| Torneios entre Decks | 3 | Baixo |

## Key Stakeholders

| Nome | Ocupação |
|---|---|
| Mariah | Product Owner |
| Matheus | Scrum Master |
| Gustavo | Tech Lead |