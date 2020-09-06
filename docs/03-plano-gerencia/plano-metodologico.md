| Data | Versão | Autor | Descrição |
|------|--------|-------|-----------|
| 2020/08/30 | 0.1 | Larissa Sales | Criação do Documento |
| 2020/09/01 | 0.2 | Letícia Araújo | Adição de Informações |
| 2020/09/01 | 0.3 | Larissa Sales | Adição de Informações |
| 2020/09/05 | 0.4 | Larissa Sales | Refinamento do Documento e inclusão da Modelagem BPMN |

# Modelagem BPMN

![](../assets/03-plano-gerencia/20200905-metodologia-larissa.png)

# 1 Papéis

## 1.1 _Scrum Master_

O _Scrum Master_ tem as seguintes responsabilidades:

- Definir, adaptar, aplicar e garantir a execução da metodologia de desenvolvimento que será utilizada na construção do produto;

- Definir métricas para analisar e melhorar a produtividade da equipe com base nos dados coletados.

## 1.2 _Product Owner_ (PO)

O PO tem as seguintes responsabilidades:

- Definir escopo do produto com base nas necessidades dos _stakeholders_;

- Definir critérios de aceitação das histórias de usuário;

- Definir e analisar métricas para garantir a entrega de valor do produto aos _stakeholders_;

- Definir proposta de valor do produto;

- Analisar custos e rentabilidade do projeto.


## 1.3 Arquiteto 

O Arquiteto tem as seguintes responsabilidades:

- Modelar e planejar a arquitetura do sistema;

- Acompanhar o desenvolvimento do produto para garantir que a arquitetura está sendo seguida.

## 1.4 _DevOps_

O _DevOps_ tem as seguintes responsabilidades:

- Definir a política de contribuição do projeto;

- Garantir o gitflow;

- Garantir a disponibilidade dos ambientes de desenvolvimento, homologação e produção;

- Garantir a integração e o deploy contínuo.


## 1.5 Desenvolvedor

O Desenvolvedor tem como responsabilidade:

- Seguir padrões e técnicas definidas;

- Seguir a metodologia e os rituais definidos pelo Scrum Master;

- Desenvolver o produto;

- Testar as soluções implementadas durante o desenvolvimento do produto.


# 2 Rituais

## 2.1 Sprints

A _Sprint_ representa um ciclo de trabalho e é realizada com o conceito de time boxing, ou seja, uma _sprint_ inicia imediatamente após a conclusão da _sprint_ anterior. Tem como objetivo a entrega de um incremento potencialmente utilizável, agregando valor ao produto.

Foi levantado em uma planilha, os horários em que os membros do time estariam disponíveis, para então especificar o cronograma das _sprints_. De acordo com esta planilha, o valor representa quantos membros estão livres em determinado horário. 

<p align="center">
    <img src="../assets/03-plano-gerencia/grade-livre.png"/>
</p>

O time utilizará um cronograma de _sprints_ semanais, com duração de 7 dias, sendo:

- Início: Segunda-feira
- Fim: Domingo

## 2.2 Revisão da _Sprint_

A Revisão da _Sprint_ consiste numa reunião formal para validar o incremento do produto produzido na _sprint_ atual e adaptar o _backlog_ do produto se necessário. 

A Revisão da _Sprint_ se dará às:
- Dia: segundas-feiras;
- Horário: 20h30.

## 2.3 Planejamento da _Sprint_

O objetivo do planejamento da _sprint_ é definir o que pode ser entregue no _sprint_ e como esse trabalho vai ser alcançado. Além disso, o _backlog_ do produto deve ser atualizado e refinado para fins de esclarecimento. O planejamento da _sprint_ deve ter no máximo duas horas.

O Planejamento da _Sprint_ se dará às:
- Dia: segundas-feiras;
- Horário: logo após a Revisão da _Sprint_.


## 2.4 _Daily_

O ritual de _Daily_ tem por objetivo trocar conhecimento acerca do que foi feito desde a última _Daily_, identificar impedimentos e priorizar o trabalho a ser realizado. Os impedimentos identificados no _Daily Scrum_ devem ser tratados pelo _Scrum Master_ o mais rapidamente possível.

As _Dailys_ serão realizadas 2 vezes por semana, às:
- Dias: quartas e sexta-feiras;
- Horário: 20h00 - 20h15.

## 2.5 Identificação de riscos

A etapa de identificação de riscos se encontra tanto no início do projeto quanto durante todo o desenvolvimento. Listar os riscos externos e internos em tabelas ou planilhas é o indicado para uma boa identificação de riscos. 

# 3 Ferramentas de planejamento

## 3.1 _Issues_

As _issues_ no Github serão utilizadas para representar todas as tarefas que a equipe realizará durante o desenvolvimento do projeto. Para a melhor entendimento dessas atividades, as _issues_ devem conter:

- Título 
    - Descrição breve e clara, com verbos no particípio, do que deverá ser feito;
    - Se cabível, seguir o padrão de Épicos e Histórias de Usuário descritos em [3.2](#_32-Épicos) e [3.3](#_33-histórias-de-usuário-us).

- Descrição

- _Label_

- Responsáveis

## 3.2 Épicos

Os Épicos definem um tema que agrupa tarefas que serão realizadas e se comporta como grandes US. No desenvolvimento do projeto, os Épicos terão o objetivo de agrupar US e deverão conter:

- Título: [EP##] Nome;

- Descrição: Eu, como [nome do ator], gostaria de [descrição sucinta];

- USs: Lista de USs atreladas ao Épico.

## 3.3 Histórias de Usuário (US)

As USs (_user stories_) são descrições de alto nível de funcionalidades que definem funcionalidades do produto vista pela perspectiva dos _stakeholders_. As USs serão documentadas no GitHub como _issues_ (que obrigatoriamente deverão estar atreladas a Épicos) e seguirão um template definido:

- Código/Nome: [US##] Nome;

- Descrição: Eu, como [nome do ator], gostaria de [descrição sucinta];

- Tarefas: Lista de atividades que levam a produção da funcionalidade;

- Critérios de aceitação: Lista de requisitos para a aceitação dessa US.

## 3.6 Kanban

Para monitorar o trabalho da equipe será utilizado dois quadros de Kanban na seção "_Projects_" do GitHub:

### 3.6.1 Roadmap da Wiki 

Quadro geral para manter o controle de atividades como: documentação, reuniões, treinamentos, estudos e etc. Este quadro será dividido em _To Do, Doing_ e _Done_.

### 3.6.2 Roadmap

Quadro de desenvolvimento para manter o controle da produção das USs. Este quadro será dividido em: _Product Backlog, Sprint Backlog, Doing, Testing_ e _Done_;

# 4 Métricas de gerenciamento

## 4.1 _Velocity_ 

O velocity é uma métrica utilizada para mensurar a capacidade de entrega do time. Essa métrica é baseada em _Story Points_ concluídos em um determinado período de tempo, no caso, as sprints. Essa medida apresenta a taxa de entrega de trabalho pela equipe e isso possibilita estimativas mais precisas de quantos _story points_ podem ser atribuídos ao time a cada _sprint_.

Inicialmente, a estimativa feita tende a não ter uma boa precisão, mas com o passar das sprints essa acurácia tende a aumentar.

## 4.2 _Burndown_

O _burndown_ é uma ferramenta utilizada para acompanhar o _pipeline_ de desenvolvimento. Ele mostra o trabalho completo em relação ao _velocity_ do projeto. Este gráfico também é utilizado no planejamento da _sprint_ para determinar quantos _story points_ podem ser concluídos nas sprints seguintes.

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

[1] GONÇALVES, Thiago. _Sprint Scrum_: o que é e como funciona? 2018. Disponível em: <<https://www.voitto.com.br/blog/artigo/sprint-scrum>>. Acesso em: 01 set. 2020.

[2] JUNCKES, Gabriel Dias; MORGADO, Paulo. Gerência de riscos em desenvolvimento de software. 2013. Universidade do Sul de Santa Catarina. Disponível em: <<https://www.devmedia.com.br/gerencia-de-riscos-em-desenvolvimento-de-software/28506>>. Acesso em: 01 set. 2020.

[3] SCHWABER, Ken; SUTHERLAND, Jeff. Um guia definitivo para o Scrum: As regras do jogo. Scrum Inc, 2013. 19 p.

[4] GEEKBOT. 4 Alternatives to Tedious, In-Person Daily Standup Meetings. 2020. Disponível em: <<https://geekbot.com/blog/alternatives-to-standup-meetings>>. Acesso em: 05 set. 2020.

[5] DESENVOLVIMENTOAGIL. Scrum. Disponível em: <<https://www.desenvolvimentoagil.com.br/scrum>>. Acesso em: 05 set. 2020.