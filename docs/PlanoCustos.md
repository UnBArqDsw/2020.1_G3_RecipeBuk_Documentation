# Plano de Custos

| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/09/01 | 0.1 | Letícia Araújo | Criação do Documento |

## Introdução

Gerenciamento de Custos e Esforços de Projetos é um conjunto de processos que tem por foco garantir que o projeto seja entregue dentro do orçamento aprovado. O gerenciamento de custos traz uma forma estruturada para planejar, estimar, determinar e controlar os custos. Dessa forma, garante que nenhuma etapa seja esquecida e proporciona a elaboração de um orçamento mais próximo da realidade. 

Desta forma, é possível conciliar os recursos financeiros que o projeto possui para finalizar, com aqueles que o patrocinador pode ou está disposto a pagar. Portanto, se o orçamento é a principal restrição sinalizada pelo patrocinador do projeto, os pontos restantes devem está alinhados com o orçamento.

A estimativa de custo é necessária durante todo o ciclo do pojeto, mas principlamente na fase inicial. É a partir desses cálculos que serão apresentadas as propostas apropriadas de negócio e será realizada a correta administração dos recursos ao longo do projeto. O método COCOMO 81 (COnstructive COst MOdel), é utilizado nesse projeto para cálculo das estivamativas de custos. 

## Modelo de Custo Construtivo (CONSTRUCTIVE COST MODEL - COCOMO)

O método de modelo de COCOMO, foi inicialmente proposto por Boehm em 1981. O COCOMO propõe-se a medir esforço, prazo, tamanho da equipe e custo envolvidos no desenvolvimento de software, tendo como premissa a dimensão do mesmo, fornecida em número de instruções-fonte. Esse método é baseado COCOMO apresenta uma série de equações
derivadas a partir do estudo de uma base de dados de 63 projetos, em sua maior parte na empresa TRW Systems. Os programas examinaram de 2.000 a 100.000 linhas de código em linguagens de programação de Assembly a PL/I. 

Para obter as equações do COCOMO foram combinados três fatores:

 - A experiência;
 - Resultados de outros modelos de estimativa de custo; 
 - A opinião subjetiva de gerentes de software experientes.

Atualmente existe duas aplicações do COCOMO, o 81 e o II. Nesse projeto é utilizado o 81. O  COCOMO pode ser aplicado em três classes de projetos:

 - Modo Orgânico: projetos simples, relativamente pequenos, com conjuntos de requisitos não tão rígidos, com equipes pequenas e experientes.
 - Modo Semidestacado: projetos intermediários (em tamanho e complexidade), com alguns requisitos rígidos e outros não tão rígidos, com níveis mistos de experiência nas equipes.
 - Modo Embutido: projetos com conjunto rígido de restrições operacionais, tanto de hardware, quanto de software.

O COCOMO é apresentado na forma de um conjunto de modelos divididos hierarquicamente em três níveis: Básico, Intermediário e Avançado. Por motivo de melhor adequação, o escolhido para realizar as estimativas é o modelo intermediário.


### COCOMO Intermediário

Adiciona fatores ao método básico como restrições de hardware, qualificação e experiência do pessoal. Está associado a um conjunto de direcionadores de custo, que incluem avaliações subjetivas do produto, do pessoal envolvido no desenvolvimento, das características e recursos do projeto, o que demonstra amplo detalhamento e capacidade mais acurada de estimativas.

O conjunto de atributos direcionadores do custo são agrupados em quatro categorias:

#### Atributos do produto:
 - Confiabilidade exigida do software;
 - Tamanho do banco de dados;
 - Complexidade do produto.
 
#### Atributos do hardware:
 - Restrições ao tempo de execução;
 - Restrições de memória;
 - Volatilidade do ambiente de máquina virtual;
 - Tempo de turnaround (tempo para completar o ciclo) exigido.

#### Atributos de pessoal:

 - Capacidade do analista;
 - Experiência em aplicações;
 - Capacidade do programador;
 - Experiência em máquina virtual;
 - Experiência com a linguagem de programação.

#### Atributos de projeto:

 - Uso de práticas modernas de programação;
 - Uso de ferramentas de software;
 - Cronograma exigido de desenvolvimento.


Cada um desses atributos deve ser classificado de acordo com uma escala que varia de “muito baixo” a “extremamente elevado” (em importância e valor). A partir desta classificação determina-se o Multiplicador de Esforço (considerando a Tabela publicada por Boehm (1981)). O produto de todos os resultados de Multiplicadores de Esforços é chamado de Fator de Ajustamento de Esforço.

    #### Inserir Imagem da Tabela pra ficar mais bonitinho
    
#### Calculo da Estimativa do Esforço
O resultado do esforço representa o valor de Pessoas/Mês O modelo COCOMO Intermediário usa a seguinte equação para a estimativa do esforço:

> E = a x S^b x fae

Onde: 

**E**: é o esforço aplicado (em pessoas-mês).
**S**: é o número (estimado) de linhas de código para o projeto (em milhares).
**a**: é um coeficiente fornecido pela Tabela.
**b**: é um expoente fornecido pela Tabela.
**fae**: é o Fator de Ajustamento do Esforço (multiplicação de cada um dos Multiplicadores de Esforço fornecidos pela Tabela).

#### Calculo da Estimativa do Tempo

Representa a quantidade de meses prevista para a conclusão do projeto:

> T = c x E^d

Onde:

**E**: é o esforço aplicado (em pessoas-mês).
**T**: é o tempo de desenvolvimento (em meses cronológicos).
**S**: é o número estimado de linhas de código em milhares (KLOC)* .
**a**: é um coeficiente fornecido pela Tabela.
**b**: é um expoente fornecido pela Tabela.
**c**: é um coeficiente fornecido pela Tabela.
**d**: é um expoente fornecido pela Tabela.

## Resultados

### Estimativa de Quantidade de Linhas de Códigos

### Estimativa de Esforço

### Estimativa de Tempo

## Referências

[1] MAGELA, Rogério. Engenharia de software aplicada: fundamentos. Rio de Janeiro: Alta Books, 2006. 

[2] WENDERLICH, Alexandre. Ferramenta de Cálculo de Estimativas de Software. 2008. 91 f. TCC (Graduação) - Curso de Ciências da Computação, Centro de Ciências Exatas e Naturais, Universidade Regional de Blumenau, Blumenau, 2008. Disponível em: http://fattocs.com/files/pt/livro-apf/citacao/AlexandreWenderlich-2008.pdf. Acesso em: 01 set. 2020.

[3] Meller, Maristela Corrêa. Modelos Para Estimar Custos De Software: Estudo Comparativo Com Softwares De Pequeno Porte. 2002. Disponível em: https://repositorio.ufsc.br/xmlui/handle/123456789/82351

[4] MASIERO, Paulo. Planejamento do Projeto. São Paulo: -, 2004. 117 slides, color. Disponível em: http://www.univasf.edu.br/~ricardo.aramos/disciplinas/ESI2009_2/PlanejamentoProjeto_Masiero.pdf. Acesso em: 01 set. 2020.

[5] ALMEIDA, Welison et al. A Monitoria. 2019. Disponível em: https://2019-2-arquitetura-desenho.github.io/wiki/extras/documento_visao/. Acesso em: 01 set. 2020.