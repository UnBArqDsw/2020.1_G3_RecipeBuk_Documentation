| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/10/23 | 1 | Luís Henrique e Eduardo Lima | Criação do Documento |

# GRASPs

Especialista é um princípio utilizado para determinar onde delegar responsabilidades. Essas responsabilidades incluem métodos, campos computados, e assim em diante.
Usando o princípio de Especialista, uma abordagem geral para atribuir responsabilidades é olhar para uma determinada responsabilidade, determinar a informação necessária para cumpri-la e depois determinar quem será o encarregado de executá-la. 
O método Especialista colocará a responsabilidade na classe com a maioria das informações necessárias para cumpri-la.

Criador é outro GRASP parecido com o especialista que é responsável por criar objetos fundamentais para o sistema.

Em nosso projeto possuímos diversos especialistas e criadores para melhor administrar as responsabilidades da aplicação, são eles:

[GRASPs no Frontend](GRASPs-frontend.md)

[GRASPs no Backend](GRASPs-backend.md)

[1] GRASP (padrão orientado a objetos). Disponível em: <<https://pt.wikipedia.org/wiki/GRASP_(padr%C3%A3o_orientado_a_objetos)>>. Acesso em: 23 Out. 2020.