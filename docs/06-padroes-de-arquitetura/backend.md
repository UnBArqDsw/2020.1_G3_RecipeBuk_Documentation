| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/17 | 0.1 | Eduardo Lima | Criação do Documento |

# Backend
Para a implementação do Backend utilizamos o Nodejs. Nodejs é um runtime assíncrono orientado a eventos em JavaScript, feito para criar aplicações network escaláveis, possuindo uma vasta variedade de frameworks, possibilitando um desenvolvimento rápido e de qualidade com a reutilização de software.

Utilizamos a reutilzação de software através de frameworks e serviços em nosso backend. São eles:

* Express: Framework de aplicação web para NodeJs, utilizado para criar API de maneira eficiente.
    * Hot-spot: Possuímos implementado em nossa aplicação o método Router do express, que possibilita a criação dinâmica de rotas HTTP
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Router.png) 
    * Frozen-spot: Inicializar uma aplicação web via Express
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Express.png)