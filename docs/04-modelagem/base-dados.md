# Banco de Dados
| Data |Versão| Autor | Descrição |
| ---- | ---- | ----- | --------- |
| 2020/09/22 | 0.1 | Samuel Pereira | Adição do ME-R |

## ME-R

### Entidades
&emsp;USER</br>
&emsp;RECIPE</br>
&emsp;RECIPE_BOOK</br>
&emsp;USER_SESSION</br>
&emsp;CATEGORY</br>
&emsp;STEP</br>
&emsp;INGREDIENT</br>


### Atributos
&emsp;USER(<u>email</u>, name, password_hash, birthdate)</br>
&emsp;RECIPE(<u>recipeId</u>, userEmail, name, time, portions)</br>
&emsp;RECIPE_BOOK(<u>bookId</u>, userEmail, title, description)</br>
&emsp;USER_SESSION(userEmail, <u>sessionId</u>, expirationDate)</br>
&emsp;CATEGORY(<u>id</u>, name)</br>
&emsp;STEP(recipeId, number, instruction)</br>
&emsp;INGREDIENT(<u>ingredientId</u>, name)</br>

### Relacionamentos
&emsp;USER - has - USER_SESSION</br>
&emsp;&emsp;Um USER pode ter múltiplas USER SESSIONS e uma USER SESSION só pode ser tida por um único USER.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;USER - owns - RECIPE</br>
&emsp;&emsp;Um USER pode possuir múltiplos RECIPES e um RECIPE só pode ser possuído por um único USER.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;USER - possess - RECIPE_BOOK</br>
&emsp;&emsp;Um USER pode possuir múltiplos RECIPE BOOKS e um RECIPE BOOK só pode ser possuído por um único USER.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;RECIPE - uses - INGREDIENT</br>
&emsp;&emsp;Um RECIPE usa um ou mais INGREDIENTS e um INGREDIENT pode ser usado em várias RECIPES.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>
</br>
&emsp;RECIPE - follows - STEPS</br>
&emsp;&emsp;Um RECIPE segue um ou mais STEPS e um STEP é seguido somente por um RECIPE.</br>
&emsp;&emsp;Cardinalidade: 1:n.</br>
</br>
&emsp;RECIPE_BOOK - contains - RECIPE</br>
&emsp;&emsp;Um RECIPE BOOK contém um ou mais RECIPES e um RECIPE pode estar contido em vários RECIPE BOOKS.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>
</br>
&emsp;CATEGORY - categorizes - RECIPE</br>
&emsp;&emsp;Uma CATEGORY pode categorizar vários RECIPES e um RECIPE pode ser categorizado por múltiplas CATEGORIES.</br>
&emsp;&emsp;Cardinalidade: n:m.</br>