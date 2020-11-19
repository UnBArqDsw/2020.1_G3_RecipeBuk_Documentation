| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/18 | 0.1 | Luís Taira | Criação do modelo do documento, adição da introdução e representação arquitetural sem diagrana de relações. |
| 2020/11/19 | 0.2 | Samuel Pereira | Adição da Visão de Caso de Uso |
| 2020/11/19 | 0.3 | Samuel Pereira | Correção de links na Visão de Caso de Uso e adição de referências |
| 2020/11/19 | 0.4 | Luís Taira | Adição da Visão Geral da Visão lógica |

# RecipeBuk
## Arquitetura
### Versão 1.7

## Sumário
## 1. Introdução
### 1.1 Finalidade
Este documento tem como finalidade fornecer uma visão geral da arquitetura do RecipeBuk, utilizando-se de diversas visões arquiteturais a fim de facilitar o entendimento dos processos e funcionamento de todo o sistema. Tem também como objetivo transmitir as decisões arquiteturais significativas tomadas em relação ao mesmo.

### 1.2 Escopo

<p align="justify">&emsp;&emsp;Através desse documento, é possível obter um melhor entendimento da arquitetura do RecipeBuk, permitindo ao leitor compreender o funcionamento de seu sistema, como também a abordagem utilizada para o seu desenvolvimento.</p>

### 1.3 Definições, Acrônimos e Abreviações
### 1.4 Referências

### 1.5 Visão Geral
<p align="justify">&emsp;&emsp;Este documento apresenta, de forma detalhada, a arquitetura, os requisitos e as decisões tomadas a respeito do RecipeBuk.</p>
<p align="justify">&emsp;&emsp;O documento está estruturado da seguinte maneira:</p>
<ul>
	<li>Histórico da Revisão: Responsável por deixar explícito cada alteração feita no documento e as informações a respeito do mesmo;</li>
	<li>Introdução: Fornece uma visão geral do documento inteiro;</li>
	<li>Representação arquitetural: Descreve qual é a arquitetura de software do sistema atual e como ela é representada;</li>
	<li>Metas e restrições da arquitetura: Descreve os requisitos e objetivos do software que têm algum impacto sobre a arquitetura;</li>
    <li>Visão de Caso de Uso: Descreve os casos de uso do sistema representando suas funcionalidades centrais; </li>
	<li>Visão Lógica: Descreve as partes significativas do ponto de vista da arquitetura do modelo de design;</li>
	<li>Visão de Processos: Descreve a decomposição do sistema em processos leves e
processos pesados;</li>
<li>Visão de Implantação: descreve uma ou mais configurações da rede física na qual o software é implantado e executado;</li>
<li>Visão de Implementação: descreve a estrutura geral do modelo de implementação, a divisão do software em camadas e os subsistemas no modelo de implementação e todos os componentes significativos do ponto de vista da arquitetura;</li>
<li>Visão de Dados: descreve a perspectiva de armazenamento de dados persistentes do sistema;</li>
<li>Tamanho e Desempenho: descreve as principais características de dimensionamento do software que têm um impacto na arquitetura, bem como as restrições do desempenho desejado;</li>
<li>Qualidade: descreve como a arquitetura do software contribui para todos os recursos (exceto a funcionalidade) do sistema.</li>
</ul>

## 2. Representação Arquitetural
### 2.1 Diagrama de Relações

<p align="justify">&emsp;&emsp;O estilo arquitetural cliente-servidor visa implementar uma aplicação dividindo-a em dois serviços, um cuja implantação distribui um módulo para os clientes, que se tornam responsáveis por sua execução e outro que tem seus processos executados em um servidor e se comunica com os clientes, geralmente por requisições HTTP.</p>

<p align="justify">&emsp;&emsp;Cada um dos serviços do RecipeBuk terá seu próprio repositório. Destacando assim, mais uma característica desse estilo arquitetural, onde cada um deles terá seu próprio ambiente, tecnologias, integração contínua e deploy.</p>

<p align="justify">&emsp;&emsp;Os serviços que serão implementados no RecipeBuk foram pensados para distribuir as responsabilidades e interesses entre o cliente e o servidor. São os serviços:</p>
<ul>
<li>Frontend;</li>
<li>Backend.</li>
</ul>

### 2.2 Representação dos Serviços

#### 2.2.1 Frontend
<p align="justify">&emsp;&emsp;O Frontend do RecipeBuk é responsavel por toda a interação com o usuário. Ele apresenta uma interface gráfica que habilita o usuário a usar todas as funções do sistema.</p>

<p align="justify">&emsp;&emsp; Interagindo com o Frontend o usuário terá acesso ao núcleo das funcionalidades do RecipeBuk, sendo elas principalmente: fazer pesquisas por receitas e adicionar os resultados aos favoritos, criar uma conta e fazer login, criar livros de receitas, adicionar, editar e remover receitas e visualizar os livros, receitas e receitas favorias.</p>


#### 2.2.2 Backend
<p align="justify">&emsp;&emsp; O Backend do RecipeBuk é o responsável pela funcionalidade das principais características do sistema. Através de requisições feitas pelo Frontend, o Backend irá realizar as pesquisas feitas pelo usuário, armazenar e editar contas de usuários, receitas, lista de favoritos e livros e realizar a autenticação de usuários.</p>

## 3. Metas e Restrições de Arquitetura

### 3.1 Restrições Tecnológicas

### 3.2 Requisitos Não Funcionais

## 4. Visão de Casos de Uso
<p align="justify">&emsp;&emsp;A documentação de caso de uso busca especificar o comportamento do sistema do ponto de vista do usuário. Todos os casos de uso produzidos se encontram disponíveis na <a href="#/04-modelagem/casos-de-uso.md">seção de modelagem da documentação</a>, sendo os que representam as funcionalidades centrais os que seguem:</p>

- [Caso de Uso 05: Criação de receita](04-modelagem/casos-de-uso/05.md)
- [Caso de Uso 06: Criação de livro](04-modelagem/casos-de-uso/06.md)
- [Caso de Uso 07: Adição de receita à livro](04-modelagem/casos-de-uso/07.md)
- [Caso de Uso 08: Favoritar receita](04-modelagem/casos-de-uso/08.md)
- [Caso de Uso 09: Pesquisa de receita](04-modelagem/casos-de-uso/09.md)


### 4.1 Realização de Casos de Uso
<p align="justify">&emsp;&emsp;Enquanto um caso de uso descreve o comportamento de uma funcionalidade do ponto de vista do usuário, ainda existe o ponto de vista da máquina, ou seja, do sistema. Ao incluir o ponto de vista da máquina no caso de uso, estamos criando uma realização de caso de uso, sendo uma documentação útil para guiar a construção de um sistema o qual consegue alcançar o comportamento desejado. Dessa forma, foram produzidos realizações de caso de uso para os casos de uso considerados representantes das funcionalidades centrais do RecipeBuk, os quais já foram mencionados anteriormente. Com o intuito de não poluir o documento de arquitetura, segue abaixo os hiperlinks para cada um das realizações de caso de uso:</p>

- [Realização de Caso de Uso 05: Criação de receita](06-padroes-de-arquitetura/realizacao-caso-de-uso/05.md)
- [Realização de Caso de Uso 06: Criação de livro](06-padroes-de-arquitetura/realizacao-caso-de-uso/06.md)
- [Realização de Caso de Uso 07: Adição de receita à livro](06-padroes-de-arquitetura/realizacao-caso-de-uso/07.md)
- [Realização de Caso de Uso 08: Favoritar receita](06-padroes-de-arquitetura/realizacao-caso-de-uso/08.md)
- [Realização de Caso de Uso 09: Pesquisa de receita](06-padroes-de-arquitetura/realizacao-caso-de-uso/09.md)

## 5. Visão Lógica
### 5.1 Visão Geral
<p align="justify">&emsp;&emsp;A interface do RecipeBuk com o usuáro é feita usando o framework Angular, que permite o uso de HTML e CSS para desenvolvimento gráfico e typescript para sua lógica e efeito para ser executado no lado do cliente. A plataforma Node.js é um ambiente de tempo de execução que executa código e javascript para realizar o processamento do RecipeBuk enquanto também é usado o framework Express.js para a exposição de rotas.</p>

### 5.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura

#### 5.2.1 Diagrama de pacotes

#### 5.2.2 Diagrama de classe

##### 5.2.2.1 Diagrama de Classe do 

### 5.4 Visão da Implantação

### 5.5 Visão da Implementação

## 6. Tamanho e Desempenho

## 7. Qualidade

## Referências
[1] SCHMIDT, David. Lecture 7: Use cases and diagrammatic realizations. Disponível em: <http://people.cs.ksu.edu/~schmidt/501s13/Lectures/Lecture07S.html>. Acesso em: 19, Novembro, 2020.</br>
[2] IBM Corp. Diretriz: Realização de Casos de Uso. Disponível em: <https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/guidances/guidelines/use-case_realization_C690D81F.html>. Acesso em: 19, Novembro, 2020.</br>
[3] IBM Corp. Artefato: Realização de Casos de Uso. Disponível em: <https://www.cin.ufpe.br/~gta/rup-vc/core.base_rup/workproducts/rup_use_case_realization_E4F713BD.html>. Acesso em: 19, Novembro, 2020.
