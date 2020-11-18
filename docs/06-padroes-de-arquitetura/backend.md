| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/17 | 0.1 | Eduardo Lima | Criação do Documento |
| 2020/11/18 | 0.2 | Samuel Pereira | Adição do Crawler |

# Backend

## NodeJS
Para a implementação do Backend utilizamos o Nodejs. Nodejs é um runtime assíncrono orientado a eventos em JavaScript, feito para criar aplicações network escaláveis, possuindo uma vasta variedade de frameworks, possibilitando um desenvolvimento rápido e de qualidade com a reutilização de software.

Utilizamos a reutilização de software através de frameworks e serviços em nosso backend. São eles:

* Express: Framework de aplicação web para NodeJs, utilizado para criar API de maneira eficiente.
    * Hot-spot: Possuímos implementado em nossa aplicação o método Router do express, que possibilita a criação dinâmica de rotas HTTP
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Router.png) 
    * Frozen-spot: Inicializar uma aplicação web via Express
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Express.png)
		
## Crawler
Crawler é um módulo para NodeJS que tem como funcionalidade a realização de Web Scraping e Web Crawling, permitindo a obtenção de informações de páginas da web de forma sistematizada. </br>

No ponto de vista de reutilização de software do Crawler no Recipebuk, a utilização do Crawler simplifica o desenvolvimento do projeto pois justamente fornece essas funcionalidades de *Web Scraping* e *Web Crawling*, a qual é utilizada no projeto para a obtenção da informações de receitas de diversos websites. A ausência desse módulo, ocasionaria na necessidade de implementação das seguintes funcionalidades:
- Obtenção de informações de páginas através de requisições HTTP;
- *Parsing* das informações adquiridas, a qual é resolvido pelo Crawler através da disponibilização do Cheerio, uma implementação simplificada do JQuery para servidores;
- Agendamento e sincronização de todas as requisições para o fornecimento da resposta do servidor, onde o Crawler soluciona através do fornecimento de uma fila de requisições a qual possui um callback quando todas as requisições são finalizadas e processadas. </br>

No projeto, o Crawler atua como uma reutilização de código de caixa-branca, pois utilizamos a funcionalidade de *scraping* para adquirir informações de outros sites - a qual temos de definir como será feita a filtragem de dados em cada um dos websites alvos - e a funcionalidade de callback de fila esvaziada - também definindo o comportamento quando a mesma é esvaziada - ambos se caracterizando como hot spots. Exemplos da utilização seguem abaixo:</br>

- Hot spot: Implementação de tratamento de dados do website TudoGostoso
 ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/crawler_data_treatment.png)
 [Crawler.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/src/models/Crawler.js)
 
 - Hot spot: Implementação de callback para retorno de resultado
 ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/getResults.png)
 [Crawler.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/src/models/Crawler.js)