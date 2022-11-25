* Vamos aprender o que são chaves primárias e chaves estrangeiras 
* Vamos ver exemplos de como usar eles para criar colunas e tabelas, porém vamos ver isso mais em detalhe na aula sobre criação de tabelas 


## O que é uma chave primária ?

*Uma chave primária é basicamente uma coluna ou grupo de colunas, usada para identificar unicamente uma linha em uma tabela 

*Você consegue criara essas chaves primárias através que restrições (ou constraints em inglês),que são regras que você define quando está criando uma coluna (DICA : é bom memorizar em inglês , constraints, pois fica mais fácil para fazer a pesquisa no banco de dados ). 
* Assim quando você faz isso você está criando um índice único para aquela coluna ou grupo de colunas 


como fazer ?

CREATE TABLE nome_Tabela (
    nomeColuna TipoDeDados PRIMARY KEY 
    nomeColuna tipoDeDados ...
)


## O que é uma chave estrangeira ? 

* Uma chave estrangeira é uma coluna ou grupo de colunas em uma tabela que identifica unicamente uma linha em outra tabela. 

* ou seja, uma chave estrangeira é definida em uma tabela onde ela é apenas uma referência e não contem todos os dados ali

* então  uma chave estrangeira é simplismente uma coluna ou grupo de colunas que é uma chave primária em outra tabela

* A tabela que contém a chave estrangeira é chamada de tabela referênciadora ou tabela filho. Ea tabela na qual a chave estrangeira é referênciada é chamada de tabela referenciada ou tabela pai 

* uma tabela pode ter mias de uma chave estrangeira dependendo do seu relacionamento com as outras tabelas

Regras básicas : 

* No SQL Server você define uma chave estrangeira atraves de um " Foreign Key Constraint " ou Restrição de chave estrangeira 

* Uma Restrição de chave Estrangeira indica que os valores em uma coluna ou grupo de colunas na tabela filho correspondem aos valores na tabela pai 

* Nos podemos entender que uma chave estrangeira mantém a " integridade referencial " 
 

 exemplo : 

 |ProductID|
 |---------|
 |ProductID|
 |ProductName|
 |SupllierID|
 | *CategoryID* |
 |QuantityPerUnit|
 |UnitPrice|
 |UnitInStock|
 |UnitOnOrder|
 |ReorderLevel|
 |Discontinued|


 |Categories|
 |---------|
 |CategoryID|
 |CategoryName|
 |Description|
 |Picture| 







