| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/14 | 1.0 | Dâmaso e Letícia | Criação do Documento |

# Estudo Dirigido - GoFs Comportamental
O modelo de comportamento se concentra no algoritmo e na atribuição de responsabilidades entre os objetos. Eles não apenas descrevem os padrões de objetos ou classes, mas também os padrões de comunicação entre os objetos. O modelo de comportamento de classe usa herança para distribuir comportamento entre classes, enquanto o modelo de comportamento de objeto usa composição de objeto como recompensa pela herança.
## Chain of Responsibility
A principal função é evitar a dependência entre um objeto receptor e um objeto solicitante. Consiste em uma série de objetos receptores e de objetos de solicitação, onde cada objetos de solicitação possui uma lógica interna que separa quais são tipos de objetos receptores que podem ser manipulados. O restante é passado para o próximo objetos de solicitação da cadeia.
### Pontos positivos
- É possível controlar a ordem de tratamento dos objetos.
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros componentes diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.

### Pontos negativos
- Alguns objetos podem acabar sem tratamento.
### Viabilidade
Não tem aplicação.

## Command
É um padrão no qual os objetos são usados ​​para encapsular todas as informações necessárias para realizar ações ou disparar eventos no futuro.
### Pontos positivos
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros componentes diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- É possível implementar execuções adiadas de operações.
- É possível combinar um conjunto de comandos simples em um complexo.
### Pontos negativos
- Uma vez que uma nova camada é introduzida entre o emissor e o receptor, o código pode se tornar mais complicado.
### Viabilidade
Não tem aplicação.
## Iterator
Iterator é um padrão de design comportamental que permite percorrer os elementos de uma coleção sem expor sua representação (lista, pilha, árvore, etc.).
### Pontos positivos
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros componentes diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- Como cada objeto iterador contém seu próprio estado de iteração, a mesma coleção pode ser iterada em paralelo.
- É possível atrasar uma iteração e continuá-la quando necessário.
### Pontos negativos
- Aplicar o padrão pode ser um preciosismo se sua aplicação só trabalha com coleções simples.
- Usar um iterador pode ser menos eficiente que percorrer elementos de algumas coleções especializadas diretamente.
### Viabilidade
Tem aplicação.

## Mediator
Este é um padrão de projeto frequentemente utilizado quando é necessário encapsular como os objetos interagem, ou seja, estabelecer comunicação entre os objetos por meio de um mediador.
### Pontos positivos
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros componentes diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- É possível reduzir o acoplamento entre os vários componentes de um programa.
- É possível reutilizar componentes individuais mais facilmente.
### Pontos negativos
- É possível que o mediator vire um God Object.
### Viabilidade
Tem aplicação.

## Memento
É um padrão de projeto que permite armazenar o estado interno de um objeto em um determinando momento, para que seja possível retorná-lo a este estado, sem que isso cause problemas com o encapsulamento.
### Pontos positivos
- O retrato do estado do objeto pode ser gerado sem violar seu encapsulamento.
- Ao permitir que o cuidador mantenha um registro histórico da identidade do originador, dessa forma o código do originador pode ser simplificado.
### Pontos negativos
- A aplicação pode consumir muita RAM se os clientes criarem mementos com muita frequência.
- Cuidadoras devem acompanhar o ciclo de vida da originadora para serem capazes de destruir mementos obsoletos.
- A maioria das linguagens de programação dinâmicas, tais como PHP, Python, e JavaScript, não conseguem garantir que o estado dentro do memento permaneça intacto.
### Viabilidade
Tem aplicação.

## Observer
 É um padrão de projeto de software que define uma dependência um-para-muitos entre objetos de modo que quando um objeto muda o estado, todos seus dependentes são notificados e atualizados automaticamente.
### Pontos positivos
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- É possível estabelecer relações entre objetos durante a execução.
### Pontos negativos
- Dependentes são notificados em ordem aleatória
### Viabilidade
Não tem aplicação.

## State
O padrão State permite que um objeto altere seu comportamento quando seu estado interno muda.
### Pontos positivos
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros componentes diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- É possível simplificar o código de contexto ao eliminar condicionais de máquinas de estado pesadas.
### Pontos negativos
- Aplicar o padrão pode ser um gasto execessivo se a máquina de estado só tem alguns estados ou raramente muda eles.

### Viabilidade
Não tem aplicação.

## Strategy
É um padrão de projeto comportamental que permite que você defina uma família de algoritmos, coloque-os em classes separadas, e faça os objetos deles intercambiáveis.
### Pontos positivos
- *Princípio aberto/fechado*. Você pode adicionar novos componentes ao código sem quebrar ou afetar os outros componentes já existentes.
- É possível trocar algoritmos usados dentro de um objeto durante a execução.
- É possível isolar os detalhes de implementação de um algoritmo do código que usa ele.
- É possível substituir a herança por composição.
### Pontos negativos
- Se há, apenas, um par de algoritmos e eles raramente mudam, não há motivo real para deixar o programa mais complicado com novas classes e interfaces.

### Viabilidade
Não tem aplicação.
## Referências Bibliográficas
[1] REFACTORING.GURU. Padrões de Projeto. Disponível em: <<https://refactoring.guru/pt-br/design-patterns>>. Acesso em: 14 nov. 2020.
