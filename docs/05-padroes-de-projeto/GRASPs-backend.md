| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/10/23 | 1 | Luís Henrique e Eduardo Lima | Criação do Documento |

# GRASPs Backend

## GRASP Criador

* User

Apesar de ser um Criador, também é o Especialista responsável por instanciar um usuário na aplicação.

![](../assets/05-padroes-de-projeto/GRASPs-back/criador-user.png)

* Crawler

Criador responsável pela criação do crawler.

![](../assets/05-padroes-de-projeto/GRASPs-back/crawler-criador.png)


## GRASP Especialista

* UserRepository

Especialista responsável por toda interação da model User com o banco de dados.

![](../assets/05-padroes-de-projeto/GRASPs-back/user-repository-especialista.png)

* UserRoutes

Especialista responsável por toda interação da model User com sistemas externos ao backend da aplicação.

![](../assets/05-padroes-de-projeto/GRASPs-back/user-routes-especialista.png)

* CrawlerRoutes

Especialista responsável por toda interação da model Crawler com sistemas externos ao backend da aplicação.

![](../assets/05-padroes-de-projeto/GRASPs-back/crawler-routes.png)