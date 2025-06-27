# Engenharia de Software

## Requisitos

### Requisitos Funcionais

| Requisito | Descrição                                                                                                  | Prioridade | Caso de Uso |
|-----------|------------------------------------------------------------------------------------------------------------|------------|-------------|
| RF01      | O sistema deve permitir o usuário criar sua própria carta personalizada.                                   | Alta       | UC01        |
| RF02      | O sistema deve permitir o usuário selecionar e avaliar uma carta de outro aluno                            | Alta       | UC02        |
| RF03      | O sistema deve permitir o usuário avaliar atributos especificos de cada aluno                              | Alta       | UC03        |
| RF04      | O sistema deve permitir o usuário se alto avaliar somente 1 vez                                            | Média      | UC04        |
| RF05      | O sistema deve fornecer um feedback geral com base em todos os feedbacks passados pelos alunos.            | Média      | UC05        |
| RF06      | O sistema deve permitir a criação de um deck com a combinação de cartas escolhidas para simular uma equipe | Média      | UC06        |
| RF07      | O sistema deve permitir a comparação entre decks(equipes)                                                  | Baixa      | UC07        |
| RF08      | O sistema deve escolher a foto da carta com base na habilidade com mais pontos do aluno.                   | Baixa      | UC08        |

### Requisitos Não Funcionais

| Requisito | Descrição                                                                                      | Prioridade | Caso de Uso |
|-----------|------------------------------------------------------------------------------------------------|------------|-------------|
| RNF01     | O sistema deve ser utilizar o serviço de usuários da opaleiros                                 | Alta       | UC08        |
| RNF02     | O sistema deve realizar o calculo dos atributos para saber a pontuação principal e sua classe. | Alta       | UC08        |
| RNF03     | O sistema deve realziar o cálculo em tempo real dos decks e suas comparações                   | Alta       | UC09        |

<br/>
<br/>

### Wireframe

> Link para o Figma do
> projeto: [Figma](https://www.figma.com/design/asYdMJ1SKlvyYvrJsAApWc/Grade-Me-Hard?node-id=0-1&t=7dpCAurvrTR54kAm-1)

### Banco de Dados

Em breve

## UML

Em breve

### Casos de Uso

#### **UC01 - Criação da própria carta**

| **Nome**             | Criação da própria carta                             |
|----------------------|------------------------------------------------------|
| **Descrição**        | O aluno pode criar a própria avaliação uma vez       |
| **Fluxo de criação** | O aluno faz seu próprio feedback                     |
| **Ator**             | Aluno                                                |
| **Pré-condições**    | O aluno deve estar matriculado para ter dados reais. |
| **Pós-condições**    | O aluno deve escolher outro aluno para avaliar.      |

#### **UC02 - Avaliar cartas de outros alunos**

| **Nome**             | Avaliar cartas de outros alunos                                   |
|----------------------|-------------------------------------------------------------------|
| **Descrição**        | O aluno seleciona a carta que deseja avaliar perante outro aluno. |
| **Fluxo de criação** | O aluno escolhe a carta para avaliar.                             |
| **Ator**             | Aluno                                                             |
| **Pré-condições**    | O sistema deve verificar se a carta existe.                       |
| **Pós-condições**    | O feedback é atualizado, juntamente com seus atributos.           |

#### **UC03 - Avaliar atributos específicos de aluno**

| **Nome**             | Avaliar atributos específicos de aluno                                           |
|----------------------|----------------------------------------------------------------------------------|
| **Descrição**        | O aluno pode avaliar atributos específicos de outros alunos durante a avaliação. |
| **Fluxo de criação** | O aluno seleciona atributos específicos e fornece uma avaliação detalhada.       |
| **Ator**             | Aluno                                                                            |
| **Pré-condições**    | O aluno deve ter selecionado uma carta para avaliar.                             |
| **Pós-condições**    | Os atributos específicos são atualizados na carta do aluno avaliado.             |

#### **UC04 - Auto avaliação única**

| **Nome**             | Auto avaliação única                                                   |
|----------------------|------------------------------------------------------------------------|
| **Descrição**        | O sistema permite que o aluno se auto avalie apenas uma única vez.     |
| **Fluxo de criação** | O aluno acessa a funcionalidade de auto avaliação e preenche os dados. |
| **Ator**             | Aluno                                                                  |
| **Pré-condições**    | O aluno não deve ter realizado auto avaliação anteriormente.           |
| **Pós-condições**    | A auto avaliação é registrada e a opção fica bloqueada para o aluno.   |

#### **UC05 - Fornecer feedback geral**

| **Nome**             | Fornecer feedback geral                                                    |
|----------------------|----------------------------------------------------------------------------|
| **Descrição**        | O sistema gera um feedback geral baseado em todas as avaliações recebidas. |
| **Fluxo de criação** | O sistema coleta todas as avaliações e gera um relatório consolidado.      |
| **Ator**             | Sistema                                                                    |
| **Pré-condições**    | O aluno deve ter recebido pelo menos uma avaliação de outros colegas.      |
| **Pós-condições**    | O feedback geral é disponibilizado para o aluno visualizar.                |

#### **UC06 - Criar deck de equipe**

| **Nome**             | Criar deck de equipe                                                                       |
|----------------------|--------------------------------------------------------------------------------------------|
| **Descrição**        | O aluno pode criar um deck combinando cartas de diferentes alunos para simular uma equipe. |
| **Fluxo de criação** | O aluno seleciona cartas de diversos alunos e as organiza em um deck.                      |
| **Ator**             | Aluno                                                                                      |
| **Pré-condições**    | Deve existir cartas disponíveis de outros alunos para seleção.                             |
| **Pós-condições**    | O deck é criado e salvo no perfil do aluno.                                                |

#### **UC07 - Comparar decks/equipes**

| **Nome**             | Comparar decks/equipes                                                   |
|----------------------|--------------------------------------------------------------------------|
| **Descrição**        | O sistema permite comparar diferentes decks criados pelos alunos.        |
| **Fluxo de criação** | O aluno seleciona dois ou mais decks e solicita a comparação.            |
| **Ator**             | Aluno                                                                    |
| **Pré-condições**    | Devem existir pelo menos dois decks criados para comparação.             |
| **Pós-condições**    | O sistema apresenta uma análise comparativa entre os decks selecionados. |

#### **UC08 - Definir foto da carta automaticamente**

| **Nome**             | Definir foto da carta automaticamente                                                                 |
|----------------------|-------------------------------------------------------------------------------------------------------|
| **Descrição**        | O sistema escolhe automaticamente a foto da carta baseada na habilidade com maior pontuação do aluno. |
| **Fluxo de criação** | O sistema analisa os atributos do aluno e seleciona a imagem correspondente.                          |
| **Ator**             | Sistema                                                                                               |
| **Pré-condições**    | O aluno deve ter pelo menos um atributo avaliado para determinar a habilidade principal.              |
| **Pós-condições**    | A foto da carta é definida automaticamente baseada na habilidade dominante.                           |

## Diagrama de sequência

Em breve