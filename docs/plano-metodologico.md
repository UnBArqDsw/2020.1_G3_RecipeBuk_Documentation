| Data | Versão | Autor | Descrição |
|------|--------|-------|-----------|
| 2020/08/30 | 0.1 | Larissa Sales | Criação do Documento |
| 2020/09/01 | 0.2 | Letícia Araújo | Adição de Informações |
| 2020/09/01 | 0.3 | Larissa Sales | Adição de Informações |

# 1 Papéis

## 1.1 Scrum Master ????

O Scrum Master as seguintes responsabilidades:

- Definir, adaptar e aplicar a metodologia de desenvolvimento que será utilizada na construção do produto;

- Definir métricas para analisar e melhorar a produtividade da equipe com base nos dados coletados;

- Garantir a execução da metodologia definida nesse documento.

## 1.2 Product Owner (PO)

O PO tem as seguintes responsabilidades:

- Definir escopo do produto com base nas necessidades dos stakeholders;

- Definir proposta de valor do produto;

- Analisar custos e a rentabilidade do projeto;

- Definir critérios de aceitação para as histórias de usuário;

- Definir e analisar métricas para garantir a entrega de valor do produto aos stakeholders.

## 1.3 Arquiteto ???? VAI TER?

O Arquiteto tem as seguintes responsabilidades:

- Modelar e planejar a arquitetura do sistema;

- Acompanhar o desenvolvimento do produto para garantir que a arquitetura está sendo seguida.

## 1.4 DevOps ???? VAI TER?

O DevOps tem as seguintes responsabilidades:

- Definir a política de contribuição para o projeto;

- Garantir o gitflow;

- Garantir a disponibilidade dos ambientes de desenvolvimento, homologação e produção;

- Garantir a integração e o deploy contínuo;


## 1.5 Desenvolvedor

O Desenvolvedor tem como responsabilidade:

- Seguir padrões e técnicas definidas;

- Seguir a metodologia e os rituais definidos pelo Scrum Master;

- Desenvolver o produto;

- Testar as soluções implementadas durante o desenvolvimento do produto.


# 2 Rituais

## 2.1 Sprints

A Sprint representa um ciclo de trabalho e é realizada com o conceito de time boxing, ou seja, uma sprint inicia imediatamente após a conclusão da sprint anterior. Tem como objetivo a entrega de um incremento potencialmente utilizável, agregando valor ao produto.

- Início: ????
- Fim: ????

## 2.2 Revisão da Sprint

A Revisão da Sprint consiste numa reunião formal para validar o incremento do produto produzido na sprint atual e adaptar o backlog do produto se necessário. No caso deste processo de desenvolvimento nem todos os stakeholders estarão presentes na revisão do incremento do produto, pois a parte interessada analisará o produto em outro momento. 

## 2.3 Planejamento da Sprint

O objetivo do planejamento da sprint é definir o que pode ser entregue no sprint e como esse trabalho vai ser alcançado. Além disso, o backlog do produto deve ser atualizado e refinado para fins de esclarecimento. O planejamento da sprint deve ter no máximo duas horas.

## 2.4 Identificação de riscos

A etapa de identificação de riscos se encontra tanto no início do projeto quanto durante todo o desenvolvimento. Listar os riscos externos e internos em tabelas ou planilhas é o indicado para uma boa identificação de riscos. 

# 3 Ferramentas de planejamento

## 3.1 _Issues_

As _issues_ no Github serão utilizadas para representar todas as tarefas que a equipe realizará durante o desenvolvimento do projeto. Para a melhor entendimento dessas atividades, as _issues_ devem conter:

- Título 
    - Descrição breve e clara, com verbos no particípio, do que deverá ser feito.

- Descrição

- Label

- Responsáveis

## 3.2 Épicos

Os Épicos definem um tema que agrupa tarefas que serão realizadas e se comporta como grandes US. No desenvolvimento do projeto, os Épicos terão o objetivo de agrupar US e deverão conter:

- Título: [EP##] Nome;

- Descrição: Eu, como [nome do ator], gostaria de [descrição sucinta];

- USs: Lista de USs atreladas ao Épico.

## 3.3 Histórias de Usuário (US)

As USs são descrições de alto nível de funcionalidades que definem funcionalidades do produto vista pela perspectiva dos stakeholders. As USs serão documentadas no GitHub como _issues_ (que obrigatoriamente deverão estar atreladas a Épicos) e seguirão um template definido:

- Código/Nome: [US##] Nome;

- Descrição: Eu, como [nome do ator], gostaria de [descrição sucinta];

- Tarefas: Lista de atividades que levam a produção da funcionalidade;

- Critérios de aceitação: Lista de requisitos para a aceitação dessa US.

## 3.6 Kanban

Para monitorar o trabalho da equipe será utilizado dois quadros de Kanban na seção "Projects" do GitHub:

### 3.6.1 Roadmap da Wiki 

Quadro geral para manter o controle de atividades como: documentação, reuniões, treinamentos, estudos e etc. Este quadro será dividido em To do, Doing e Done.

### 3.6.2 Roadmap

Quadro de desenvolvimento para manter o controle da produção das USs. Este quadro será dividido em: Product Backlog, Sprint Backlog, Doing, Testing e Done;

# 4 Métricas de gerenciamento

## 4.1 _Velocity_ 

O velocity é uma métrica utilizada para mensurar a capacidade de entrega do time. Essa métrica é baseada em _Story Points_ concluídos em um determinado período de tempo, no caso, as sprints. Essa medida apresenta a taxa de entrega de trabalho pela equipe e isso possibilita estimativas mais precisas de quantos _story points_ podem ser atribuídos ao time a cada sprint.

Inicialmente, a estimativa feita tende a não ter uma boa precisão, mas com o passar das sprints essa acurácia tende a aumentar.

## 4.2 _Burndown_

O _burndown_ é uma ferramenta utilizada para acompanhar o _pipeline_ de desenvolvimento. Ele mostra o trabalho completo em relação ao _velocity_ do projeto. Este gráfico também é utilizado no planejamento da sprint para determinar quantos _story points_ podem ser concluídos nas sprints seguintes.

# 5 Técnica de programação

## 5.1 Programação em pares

A programação em pares (_pair programing_) é uma prática utilizada na metodologia _Extreme Programing_ (XP), na qual um par de desenvolvedores se torna responsável por produzir uma funcionalidade (entregar uma _issue_). 

Existem dois papeis: o do piloto, que codifica; e o do co-piloto, que acompanha e auxilia o piloto. Ambos os desenvolvedores devem trabalhar ao mesmo tempo e no mesmo computador, sendo obrigatória a inversão periódica dos papeis durante o desenvolvimento de cada funcionalidade.

# 6 Comunicação

As principais ferramentas de comunicação da equipe serão:

- Telegram
    - O grupo no Telegram será utilizado para garantir uma comunicação rápida entre os membros da equipe;

- Microsoft Teams
    - Esta plataforma será o principal canal para a realização de reuniões;

- Google Drive
    - Haverá uma pasta no Google Drive para o compartilhamento de documentos e artefatos;

- Github
    - O GitHub será a principal ferramenta para documentar as tarefas (em forma de _issues_) e os responsáveis por elas;
    
    - Será utilizada também para adicionar comentários, dentro de cada _issue_, para tirar dúvidas ou fazer considerações;

# 7 Referências 

[1] GONÇALVES, Thiago. Sprint Scrum: o que é e como funciona? 2018. Disponível em: https://www.voitto.com.br/blog/artigo/sprint-scrum. Acesso em: 01 set. 2020.

[2] JUNCKES, Gabriel Dias; MORGADO, Paulo. Gerência de riscos em desenvolvimento de software. 2013. Universidade do Sul de Santa Catarina. Disponível em: https://www.devmedia.com.br/gerencia-de-riscos-em-desenvolvimento-de-software/28506. Acesso em: 01 set. 2020.

[3] SCHWABER, Ken; SUTHERLAND, Jeff. Um guia definitivo para o Scrum: As regras do jogo. Scrum Inc, 2013. 19 p.