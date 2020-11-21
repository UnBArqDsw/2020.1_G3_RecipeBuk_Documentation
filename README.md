<p align="center">
    <img src="docs/assets/assets/logo.svg" alt="Logo RecipeBuk" width='50%'/>
</p>

# RecipeBük

Toda a nossa documentação está disponível para visualização em: http://www.recipebukdocs.tk/

Este é o nosso repositório de documentação. Se você quiser conferir os códigos do nosso sistema, nós temos o repositório de [Frontend](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Frontend) e o repositório de [Backend](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend).

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


## Screenshots
![](https://i.imgur.com/F0bQZNf.png)
![](https://i.imgur.com/BY6b1uF.png)
![](https://i.imgur.com/OgmJBLp.png)
![](https://i.imgur.com/XYAA1el.png)



## Instalação 
**Linguagens**: Typescript, Javascript, yaml<br>
**Tecnologias**: Angular, Nodejs, Docker<br>
Possuir Docker e Docker-compose instalados, assim como make(build-essencials)

## Uso 
Para exceutar o projeto realize o clone do repositório de Backend e Frontend.

Comando para executar Frontend: `make dev`

Comando para executar Backend: `make up-build`

O projeto estará disponível no enedereço localhost:4200

## Vídeo
Adicione 1 ou mais vídeos com a execução do projeto final.

## Outros 
Link para utilizar o software: http://ec2-18-228-7-121.sa-east-1.compute.amazonaws.com:4200/

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
- `dev`: versão de desenvolvimento que servirá como base para as demais _branches_ (se aplica apenas aos repositórios de [Frontend](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Frontend) e de [Backend](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend));

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
