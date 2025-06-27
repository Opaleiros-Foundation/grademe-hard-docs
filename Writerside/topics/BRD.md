# BRD

> **Definição de BRD**
>
> A business requirements document (BRD) é um relatório detalhado que descreve tudo o que um novo projeto requer para
obter sucesso. Este documento delineia os objetivos do projeto, o que é esperado ao longo do ciclo de vida do projeto e
o que é necessário para alcançar o projeto.
>
{style="note"}



## Objetivo do projeto

Um sistema para avaliar e analisar profissionalmente e acadêmicamente comparar a performance dos alunos em relação aos
seus colegas.
O objetivo deste projeto é criar uma plataforma onde alunos possam avaliar as atividades dos outros alunos, os quais já
trabalharam juntos e compará-las
com outras turmas ou até mesmo com outras escolas. A avaliação será feita por meio de atributos pré-definidos como:

- Comunicação
- Trabalho em Equipe
- Objetivo: Falador (Fala de tudo menos do assunto principal da daily)
- Colaboração

Esses atributos serão aplicados às atividades dos alunos. Os resultados da avaliação serão exibidos na forma de gráficos
utilizando cartas que representam o aluno com o valor de seus atributos,
permitindo que os alunos façam análises mais detalhadas sobre o desempenho dos alunos e saibam sobre o desempenho dos
seus colegas, os quais estão trabalhando em equipe junto a você.  Além de suas próprias habilidades.

## Escopo do projeto

### Objetivo principal do projeto

Implementar um sistema web que permita a avaliação entre alunos em forma de cartas de baralho.

**Funcionalidades incluídas**

- Cadastro e login de usuários
- Criação do próprio card
- Avaliação de outros cards
- Cada card terá atributos com pountuação, que será calculada com base na pontuação dada durante os feedbacks
- Simulação de equipes com outros alunos
- Comparação de equipes com base nos cards
- Batalha entre equipes e alunos
- Rank de melhores alunos e melhores equipes
- Ranking geral das escolas

**Regras que impactam o desenvolvimento.**

- Cada aluno só pode criar sua própria carta
- Um aluno só pode avaliar outra carta uma vez
- Uma carta só pode ser avaliada uma vez por aluno
- As avaliações são anônimas

**Sistemas envolvidos**

User service Opaleiros

**Usuários envolvidos**

Alunos da instituição


**Restrições técnicas ou operacionais**

o sistema deve rodar em navegadores modernos. E não será totalmente online e web.

**Premissas do projeto**

Os dados dos alunos serão gerados pelo proprio aluno.

**O que está fora do escopo (out of scope)**

O que não foi incluido no escopo do projeto.

## Requerimento de negócios

> Mvp 1.0

| Requisito de Negócio                        | Prioridade | Nível Crítico |
|---------------------------------------------|------------|---------------|
| Criação da própria carta                    | 1          | critico       |
| Avaliação de outras cartas                  | 1          | critico       |
| Atualização dos atributos das outras cartas | 1          | critico       |
| Rank de alunos                              | 1          | critico       |
| Simulação de equipes                        | 2          | medio         |
| Comparação de equipes                       | 2          | medio         |
| Batalha entre equipes                       | 2          | medio         |
| Ranking geral das equpes                    | 3          | baixo         |

## Key Stakeholders

| Nome    | Ocupação                                |
|---------|-----------------------------------------|
| Mariah  | Ditadora da Republica popular da Coreia |
| Matheus | Vigilante noturno                       |
| Gustavo | Techlead                                |

