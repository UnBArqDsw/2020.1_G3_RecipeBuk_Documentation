<p align="center">
    <img src="docs/assets/assets/logo.svg" alt="Logo RecipeBuk" width='50%'/>
</p>

# RecipeBük

Toda a nossa documentação está disponível para visualização em: http://www.recipebukdocs.tk/

**Número da Lista**: 03<br>
**Conteúdo da Disciplina**: FGA0208 - T01<br>

## Alunos
|Matrícula | Aluno |
| -- | -- |
| 17/0031438 | Dâmaso Júnio Pereira Brasileo |
| 17/0102343 | Eduardo Vieira Lima |
| 16/0130883 | Larissa Siqueira Sales |
| 15/0135939 | Letícia Karla Soares Rodrigues de Araújo |
| 17/0109208 | Luís Henrique Pereira Taira |
| 17/0114040 | Samuel de Souza Buters Pereira |

## Sobre 
O **RecipeBük** é uma aplicação de armazenamento, busca e compartilhamento de receitas culinárias. A ideia é que seja possível a todos cadastrar as suas próprias receitas e mantê-las a salvo. 

<!---
## Screenshots
Adicione 3 ou mais screenshots do projeto em termos de interface e funcionamento.

## Instalação 
**Linguagens**: xxxxxx<br>
**Tecnologias**: xxxxxx<br>
Descreva os pré-requisitos para rodar o seu projeto e os comandos necessários.
Insira um manual ou um script para auxiliar ainda mais.

## Uso 
Explique como usar seu projeto caso haja algum passo a passo após o comando de execução.

## Vídeo
Adicione 1 ou mais vídeos com a execução do projeto final.

## Outros 
Quaisquer outras informações sobre seu projeto podem ser descritas abaixo.
-->

## Políticas de Contribuição

### Commits

- Os _Commits_ devem ser escritos em inglês;

- Devem ser curtos e objetivos;

- Devem iniciar com verbo no passado;

- Devem ser compostos por:

```
    [#numero-da-issue] Mensagem
```

#### Exemplo:

```
    [#20] Implemented new text box
```

### Branches

As _branchs_ são baseadas no modelo de GitFlow e são dividas em:

- `master`: aplicação em sua versão estável;
- `dev`: versão de desenvolvimento que servirá como base para as demais _branches_.

Para a criação de uma nova _branch_, deve-se criá-la a partir da `dev` e manter o seguinte padrão:

- Os nomes das _branches_ deverão ser compostos por:

```
        numero-da-issue-nome-da-issue
```

#### Exemplo:

```
        20-criacao-da-tela-de-cadastro-de-receitas
```

### Pull Requests

- Os PRs devem ser criados a partir do **template** do repositório;

- Os PRs devem englobar as modificações necessárias para **apenas** uma _issue_;

- O _merge_ das _branches_ criadas a partir da `dev` **nunca** deverá ser feito na `master`;

- Após o _merge_, se a _branch_ não tiver mais uso, ela deverá ser **apagada**.