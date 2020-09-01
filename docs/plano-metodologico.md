| Data | Versão | Autor | Descrição |
|------|--------|-------|-----------|
| 2020/08/30 | 0.1 | Larissa Sales | Criação do Documento |
|2020/09/01 | 0.2 | Letícia Araújo | Adição de Informações |

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

## 1.3 Arquiteto

O Arquiteto tem as seguintes responsabilidades:

- Modelar e planejar a arquitetura do sistema;

- Acompanhar o desenvolvimento do produto para garantir que a arquitetura está sendo seguida.

## 1.4 DevOps

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
A Sprint Scrum representa um ciclo de trabalho e é um time-boxed, ou seja, uma sprint inicia imediatamente após a conclusão da sprint anterior. E tem o objetivo de entregar um incremento potencialmente utilizável do produto onde algum valor é acrescentado a um produto em desenvolvimento.

## 2.2 Revisão da Sprint
Uma reunião formal para validar o incremento do produto produzido na sprint atual e adaptar o backlog do produto se necessário. No caso deste processo de desenvolvimento nem todos os stakeholders estarão presentes na revisão do incremento do produto, pois a parte interessada analisará o produto em outro momento. 

A Revisão da Sprint terá as seguintes características:

- Duração de 1 hora;
- Presença de toda a equipe.

## 2.3 Planejamento da Sprint
O objetivo do planejamento do sprint é definir o que pode ser entregue no sprint e como esse trabalho vai ser alcançado. Além disso o backlog do produto deve ser atualizado e refinado para fins de esclarecimento. O planejamento do sprint deve ter no máximo de duas horas.

- Duração: 7 dias.
- Início: Segunda-feira, 10 horas da manhã.
- Final: Domingo, 12 horas.

## 2.4 Identificação de riscos

A etapa de identificação de riscos se encontra tanto no início do projeto quanto durante todo o desenvolvimento. Listar os riscos externos e internos em tabelas ou planilhas é o indicado para uma boa identificação de riscos. Nesse projeto, a equipe identifica e lista os riscos internos e externos da sprint.

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

## 4.1 Velocity ????

O velocity é uma medida de story points concluídos em um determinado período de tempo, no caso desse projeto o tempo seria as sprints semanais. Essa medida apresenta a taxa de entrega de trabalho pela equipe e isso possibilita estimativas mais acuradas de story points que podem ser atribuídos ao time por sprint.

Inicialmente a estimativa feita pode não ser tão acurada, mas com o passar das sprits essa acurácia tende a aumentar.

## 4.2 Burndown
O burndown mostra o trabalho que está completo relacionado com o velocity do projeto. O gráfico de burndown mostra como as projeto está andando, o que apresenta uma boa noção de quantos story points podem ser realizados em uma determinada sprint [4].

# 5 Técnica de programação

## 5.1 Programação em pares

A programação em pares (_pair programing_) é uma prática extraída da metodologia _Extreme Programing_ (XP), na qual um par de desenvolvedores se torna responsável por produzir uma funcionalidade. 

Existem dois papeis: o do piloto, que codifica; e o do co-piloto, que acompanha e auxilia o piloto. Ambos os desenvolvedores devem trabalhar ao mesmo tempo e no mesmo computador, sendo obrigatória a inversão periódica dos papeis durante o desenvolvimento de cada funcionalidade.

Ao decorrer do projeto, o Scrum Master será responsável por redefinir os pares do Time de Desenvolvimento a cada sprint para garantir a homogeneidade da equipe.

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