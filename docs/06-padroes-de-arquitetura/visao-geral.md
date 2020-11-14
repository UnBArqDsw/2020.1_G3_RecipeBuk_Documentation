| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/11/14 | 1.0 | Dâmaso Júnio e Letícia Karla Araújo | Criação do Documento|
 
# Arquitetura de Software

## Arquitetura Monolítica
Uma das arquiteturas mais indicadas para aplicações Web devido a sua simplicidade. Tem como características:

* Pode suportar diferentes tipos de cliente como desktop/mobile;
* Pode exportar APIs para comunicação com outros serviços;
* Pode integrar outras aplicações utilizando serviços REST/SOAP ou filas de mensagens, como por exemplo a fila SQS da AWS;
* Pode tratar requisições HTTP, executar regras de negócio, acessar banco de dados e trocar informações com outros sistemas;
* Podem escalar verticalmente aumentando o poder das máquinas em que a aplicação roda ou horizontalmente com a adição instâncias atrás de um Load Balancer.

### Vantagens:
* Maior facilidade de desenvolvimento — principalmente pela uniformidade do stack de tecnologias entre todos os layers;
* Mais simples para testar já que toda a aplicação é entregue em um único pacote, o que facilita testes de integração e end-to-end;
* Mais simples e rápido para efetuar o deploy, já que temos um único pacote para se preocupar;
* Mais simples de se escalar com instâncias atrás de um Load Balancer;
* Necessita de um time menor para manter a aplicação;
* Os desenvolvedores compartilham de um conhecimento equalizado, já que trata-se de um único codebase;
* O stack é mais simples e fácil de aprender;
* O desenvolvimento inicial é mais rápido, facilitando o time to market;
* Precisa de uma infraestrutura simples. Algumas vezes um simples container ou JVM é o suficiente. 

### Desvantagens:
* Os componentes tem alto acoplamento, o que resulta em efeitos colaterais como regressão de problemas devido a atualização;
* Tende a se tornar complexo e gigante depois de certo tempo, aumentando o tempo de desenvolvimento. Novas funcionalidades vão demorar mais para serem desenvolvidas e o refactor será cada vez mais complexa devido ao alto acoplamento;
* A aplicação toda precisa de um deploy para adição de qualquer feature;
* É menos confiável devido ao acoplamento dos módulos. Um pequeno problema em um serviço não muito importante pode quebrar a aplicação toda;
* A adoção de novas tecnologias é difícil e geralmente toda a aplicação precisa ser migrada o que geralmente resulta em um stack defasado a longo prazo;
* Serviços críticos não podem ser escalados individualmente o que aumenta o uso de recursos;
* Tempo longo de inicialização e grande utilização de CPU e memória;
* As equipes serão mais interdependentes e será desafiador escalar as equipes.

## Arquitetura Distribuída
A Arquitetura Distribuída tem como características:
* Servidores de serviços compartilhados (ex. arquivos, impressão),
com boa capacidade de processamento;
* Estações de trabalho com bom poder de processamento, rodando
aplicações locais, e sendo acessadas via interfaces gráficas;
* Redes com boa velocidade.

### Vantagem:
* Facilidade de gerência, seja em termos de segurança, controle de usuários e de aplicações.

### Desvantagens:
* Interface com usuário é limitada;
* Usuário não tem autonomia;
* Depedência do fornecedor, pos as arquiteturas de hardware, software e comunicação são privadas;
* Processamento Centralizado, o que dificulta a escabilidade;
* Alto custo de manuntenção e evolução.

## Referências Bibliográficas

[1]  GERTEL, Lucas. Padrões de Arquitetura Web: monolítica ou micro serviços?. Monolítica ou Micro Serviços?. 2019. Disponível em: <<https://medium.com/@lgertel/padr%C3%B5es-de-arquitetura-web-monol%C3%ADtica-ou-micro-servi%C3%A7os-7b3f0c9394fe>>. Acesso em: 14 nov. 2020.

[2] SERRANO, Milene. Arquitetura e Desenho de Software: estilos e padrões arquiteturais i. ESTILOS E PADRÕES ARQUITETURAIS I. Disponível em: <<https://aprender3.unb.br/pluginfile.php/26819/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Estilos%20e%20Padr%C3%B5es%20Arquiteturais%20I%20-%20Profa.%20Milene.pdf>>. Acesso em: 14 nov. 2020.