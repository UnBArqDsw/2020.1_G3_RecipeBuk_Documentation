| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/10/24 | 0.1 | Samuel | Implementação do GOF - Estrutural (Composite)|
| 2020/11/14 | 1.0 | Dâmaso e Letícia | Criação do Documento |

# Estudo Dirigido - GoFs Estrutural

## Adapter

O **Adapter** permite que objetos com interfaces incompatíveis possam trabalhar conjunto.

Geralmente esse tipo de padrão de projeto é utilizado quando é necessário acessar alguma biblioteca útil ou legado que seja necessária a utilização no projeto, porém essa biblioteca é incompatível com os tipos de dados que são apresentados dentro do software.

1. É criado uma classe de interface para o  `Client` que descreve o que é necessário para outras classes funcionarem com o meu código já existente.
2. É criado uma classe `Adapter` para que essa possa fazer a conexão com o serviço ou biblioteca a qual eu necessito utilizar para alterar as estruturas dos meus dados dentro do projeto.
3. Por fim, a biblioteca ou serviço externo é conectado ao meu `Adapter` para que ela possa se comunicar com o resto do meu software

![](imagem da implementação do Adapter)

### Pontos positivos

- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros adaptadores diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos adaptadores ao código sem quebrar ou afetar os clientes ou adaptadores já existentes.

### Pontos negativos

- A complexidade do código aumenta bastante pela quantidade de interfaces e classes que tendem a ser criadas para plena adaptação de todos os problemas, sendo mais simples a implementação de mudanças dentro das classes ou serviços. Mantendo um pouco da qualidade do software.

### Aplicação

Foi utilizado no backend do projeto, a biblioteca `Crawler` que é reponsável por buscar receitas em sites de terceiros como se fosse um web-crawler mesmo que faz a varredura em outros sites e busca por conteúdos pré-definidos. 
A forma da implementação aconteceu dentro da classe, onde precisavámos adaptar o dado recebido pela biblioteca para o dado que nós iríamos mostrar ao usuário.

![](foto da classe de implementação do crawler)

## Bridge

O **Bridge** é um padrão que arquitetura que divide o desenvolvimento de uma grande classe em duas hierarquias, abstração e implementação fazendo com que elas funcionem uma independente da outra.

Exemplo: Suponhamos que em um restaurante seja servido comida italiana e japonesa e são utilizamos pratos redondos e quadrados. Caso fossemos implementar classes concretas para cada prato do restaurante, teríamos 4 opções, Italiana em Prato Quadrado, Japonesa em Prato Redondo... e assim por diante. Caso queira adicionar um novo tipo de comida, vai ser necessário mais algumas classes para adequar tudo que é necessário e essa adição acontece exponencialmente. Com o **Bridge** temos podemos dividir esse problema em duas classes de Abstração e Implementação. No caso a abstração seria o Prato, e a implementação seria a Comida. Caso queira agora adicionar novos elementos é necessário apenas adicionar novas hierarquias dentro das duas classes de Prato e Comida.

1. É criado uma classe de Abstração que define a lógica de controle de alto nível
2. É criado uma classe de Implementação que define quais vão ser as implementações que pertencem à classe de Abstração.
3. É criado então subclasses referentes à implementação e abstração, fazendo com que o código se divida de forma coesa.

### Pontos positivos

- È possível criar interfaces e plataformas independentes dos sistemas operacionais
- O código não fica exposto à detalhes de implementação pois ele fica exposto apenas à abstrações de alto nível.
- *Princípio de responsabilidade única*. Você pode realizar a manutenção do código sem afetar os outros adaptadores diretamente.
- *Princípio aberto/fechado*. Você pode adicionar novos adaptadores ao código sem quebrar ou afetar os clientes ou adaptadores já existentes.

### Pontos negativos

- Ao aplicar o padrão de uma classe altamente coesa, o código tende a ficar cada vez mais complexo.

### Aplicação

Esse padrão não foi aplicado ao projeto por falta de escopo para aplicação de tal padrão. Sendo algo que pode ser muito escalável e que não se aplica ao nosso projeto.


## Referências