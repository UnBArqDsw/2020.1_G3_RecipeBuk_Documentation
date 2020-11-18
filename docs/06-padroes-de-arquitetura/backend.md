| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/17 | 0.1 | Eduardo Lima | Criação do Documento |
| 2020/11/17 | 0.2 | Larissa Sales | Adição de descrição e Referências |
| 2020/11/17 | 0.3 | Eduardo Lima | Adição de links para arquivos citados |
| 2020/11/17 | 0.4 | Eduardo Lima | Adição do tópico getUser |

# Reutilização de Software - Backend

## Node.js

Para a implementação do Backend utilizamos o Nodejs. Nodejs é um runtime assíncrono orientado a eventos em JavaScript, feito para criar aplicações network escaláveis, possuindo uma vasta variedade de frameworks, possibilitando um desenvolvimento rápido e de qualidade com a reutilização de software.

Utilizamos a reutilização de software através de frameworks e serviços em nosso backend. São eles:

## Express 

Framework de aplicação web para NodeJs, utilizado para criar API de maneira eficiente.

* Hot-spot: Possuímos implementado em nossa aplicação o método Router do express, que possibilita a criação dinâmica de rotas HTTP

    ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Router.png)

    [Router.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/src/routes/Router.js)

* Frozen-spot: Inicializar uma aplicação web via Express
        
    ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Express.png)

    [index.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/index.js)


## getUser

getUser é um método existente no repositório [UserRepository.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/src/Repository/UserRepository.js), sendo aplicado como um serviço de autenticação reutilizado em todo o Backend. Sua função é lidar com a verificação do token de autenticação do usuário , além de retornar suas informações. Atua como Frozen-spot.

![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/getUser.png)

Exemplo de aplicação no arquivo [BookRoutes.js](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Backend/blob/dev/src/routes/BookRoutes.js)

# Referências

[1] Introdução Express/Node. Disponível em: <<https://developer.mozilla.org/pt-BR/docs/Learn/Server-side/Express_Nodejs/Introdu%C3%A7%C3%A3o>>. Acesso em: 17 nov. 2020.