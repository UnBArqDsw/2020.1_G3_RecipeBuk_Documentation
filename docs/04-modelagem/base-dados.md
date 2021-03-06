
# Base de Dados
| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/09/22 | 0.1 | Samuel Pereira | Adição do ME-R |
| 2020/09/23 | 0.2 | Samuel Pereira | Atualizações do ME-R e adição do DE-R |
| 2020/09/23 | 0.3 | Samuel Pereira | Atualizações do DE-R, adição do Diagrama Lógico e mudança de título |
| 2020/09/23 | 1.0 | Samuel Pereira | Adição de visibility em RECIPE_BOOK |
| 2020/09/24 | 1.1 | Samuel Pereira | Modificação do nome de tabela USER |
| 2020/11/05 | 1.2 | Samuel Pereira | Modificação na base de dados |
| 2020/11/20 | 2.0 | Samuel Pereira | Modificação na base de dados |

## ME-R

### Entidades
&emsp;USER_ACCOUNT</br>
&emsp;RECIPE</br>
&emsp;RECIPE_BOOK</br>
&emsp;USER_SESSION</br>
&emsp;CATEGORY</br>
&emsp;FAVORITE</br>
&emsp;INGREDIENT</br>


### Atributos
&emsp;USER_ACCOUNT(<u>email</u>, name, password)</br>
&emsp;RECIPE(<u>recipeId</u>, userEmail, name, time, portions, visibility, steps)</br>
&emsp;RECIPE_BOOK(<u>bookId</u>, userEmail, title, description, visibility)</br>
&emsp;USER_SESSION(userEmail, sessionId, expirationDate)</br>
&emsp;CATEGORY(<u>idCategory</u>, name)</br>
&emsp;FAVORITE(userEmail, recipeLink, recipeImage, recipeTitle)</br>
&emsp;INGREDIENT(<u>ingredientId</u>, name)</br>

### Relacionamentos
&emsp;USER_ACCOUNT - has - USER_SESSION</br>
&emsp;&emsp;Uma USER ACCOUNT pode ter múltiplas USER SESSIONS e uma USER SESSION só pode ser tida por uma única USER ACCOUNT.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;USER_ACCOUNT - owns - RECIPE</br>
&emsp;&emsp;Uma USER ACCOUNT pode possuir múltiplos RECIPES e um RECIPE só pode ser possuído por uma única USER ACCOUNT.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;USER_ACCOUNT - possess - RECIPE_BOOK</br>
&emsp;&emsp;Uma USER ACCOUNT pode possuir múltiplos RECIPE BOOKS e um RECIPE BOOK só pode ser possuído por uma única USER ACCOUNT.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;RECIPE - uses - INGREDIENT</br>
&emsp;&emsp;Um RECIPE usa um ou mais INGREDIENTS e um INGREDIENT pode ser usado em várias RECIPES.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>
</br>
&emsp;USER_ACCOUNT - adds - FAVORITE</br>
&emsp;&emsp;Uma USER_ACCOUNT pode adicionar vários FAVORITES e um FAVORITE é adicionado somente por uma USER_ACCOUNT.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;RECIPE_BOOK - contains - RECIPE</br>
&emsp;&emsp;Um RECIPE BOOK contém um ou mais RECIPES e um RECIPE pode estar contido em vários RECIPE BOOKS.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>
</br>
&emsp;CATEGORY - categorizes - RECIPE</br>
&emsp;&emsp;Uma CATEGORY pode categorizar vários RECIPES e um RECIPE pode ser categorizado por múltiplas CATEGORIES.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>

## DE-R
![](../assets/04-modelagem/20201120-der.png)

## Diagrama Lógico
![](../assets/04-modelagem/20201120-logico.png)