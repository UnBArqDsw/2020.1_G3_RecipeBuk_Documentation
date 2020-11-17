| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/16 | 0.1 | Eduardo, Samuel e Luis | Criação do Documento |
| 2020/11/16 | 0.2 | Eduardo | Adição da introdução, referências bibliográficas e Backend |
| 2020/11/17 | 0.3 | Luis | Adição do documento de Docker |

# Reutilização de Software

A reutilização de software é uma abordagem de desenvolvimento que visa maximar o reúso de softwares existentes. O objetivo é alcançar menores custos de produção e manuntenção de software, entregas mais rápidas e maior qualidade.
A reutilização de software é comumente aplicada através de frameworks, bibliotecas, plugins, serviços, componentes e Linhas de Produto.


* [Frontend](06-padroes-de-arquitetura/frontend.md)

* [Backend](06-padroes-de-arquitetura/backend.md)

Utilizamos a reutilzação de software através de frameworks e serviços em nosso backend. São eles:

* Express: Framework de aplicação web para NodeJs, utilizado para criar API de maneira eficiente.
    * Hot-spot: Possuímos implementado em nossa aplicação o método Router do express, que possibilita a criação dinâmica de rotas HTTP
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Router.png) 
    * Frozen-spot: Inicializar uma aplicação web via Express
        ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/Express.png)

* [Docker](06-padroes-de-arquitetura/docker.md)



## Referências Bibliográficas:

[1] SERRANO, Milene. Arquitetura e Desenho de Software: REUTILIZAÇÃO & FRAMEWORK. Disponível em: <<https://aprender3.unb.br/pluginfile.php/26821/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Reutiliza%C3%A7%C3%A3o%20%20Framework%20-%20Profa.%20Milene.pdf>>. Acesso em: 16 nov. 2020.

[2] SOMMERVILLE, Ian. Engenharia de Software, 9ª Edição. Pearson Education, 2011.