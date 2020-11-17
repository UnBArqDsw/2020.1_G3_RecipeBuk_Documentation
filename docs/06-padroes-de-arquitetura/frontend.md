| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/17 | 0.1 | Samuel Pereira | Criação do documento e inclusão do Angular |

# Reutilização de Software - Frontend

## Angular
&emsp;&emsp;&emsp;&emsp;Angular é um framework de código-aberto para desenvolvimento de aplicações web baseado em Typescript, utilizando-se de uma arquitetura de hierarquia de componentes. </br>
&emsp;&emsp;&emsp;&emsp;No ponto de vista de reutilização de software do Angular no Recipebuk, a utilização do Angular nos poupa da implementação de funcionalidades como também simplifica a utilização das mesmas, esses sendo:
 - Implementação e facilitação da criação de elementos e páginas dinâmicas;
 - Implementação da sincronização de mudanças dos dados apresentados na view do cliente com a camada de dados do cliente e vice-versa;
 - Implementação de uma série de funcionalidades fornecidas como serviços.
 
 &emsp;&emsp;&emsp;&emsp;O framework Angular atua como uma reutilização de código de caixa-cinza, apresentando frozen spots - como os serviços que estão a disposição do usuário - e hot spots - como a arquitetura de componentes, a qual permite que o desenvolvedor crie os seus próprios componentes, como também a criação de serviços além dos serviços já nativos do Angular - apresentados com exemplo abaixo:
 - Hot spot: Implementação de componente Homepage
 ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/HomepageComponent.png)
 [homepage.component.ts](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Frontend/blob/dev/src/app/homepage/homepage.component.ts)
 - Frozen spot: Utilização de serviço HttpClient
 ![](../assets/06-padroes-de-arquitetura/reutilizacao-de-software/HttpClient.png)
  [homepage.component.ts](https://github.com/UnBArqDsw/2020.1_G3_RecipeBuk_Frontend/blob/dev/src/app/homepage/homepage.component.ts)
 