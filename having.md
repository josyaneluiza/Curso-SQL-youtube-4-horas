O HAVING É BASICAMENTE MUITO USADO EM JUNÇÃO COM O GRUPO BY PARA FILTRAR RESULTADOS DE UM AGRUPAMENTO . 

de forma mais simples eu gosto de entender ele como basicamente um whre para dados agrupados 

SELECT coluna1, funcaoAgregacao(coluna2)
FROM nomeTabela
GROUP BY coluna1
HAVING condicao

A grande diferença entre HAVING E WHERE é que o group by é aplicado depois que os dados já foram agrupados , enquanto o WHERE é aplicado antes dos dados serem agrupados. 

Vamos dizer que queremos saber quais nomes no sistema tem uma ocorrencia maior que 18 vezes 

SELECT FirstName, count (FirstName) as "quantidade" 
FROM Person.Person 
GROUP BY FirstName
HAVING count (firstname)>10 

Por exemplo, queremos saber quais produtos que no total de vendas estão entre 162k a 500k

SELECT productid, sum (linetotal) as "total"
FROM Sales.SalesOrderDetail
GROUP BY ProductID
HAVING SUM (linetotal) between 162000 ans 500000


USANDO O WHERE E O HAVING NA MESMA PESQUISA USANDO O EXEMPLO  : 

Voce quer saber quais nomes no sistema tem uma ocorrencia maior que 10 vezes, porem somente onde o título é Mr. 

SELECT FirstName, count(FirstName)as "quantidade"
FROM person.Person
WHERE Title= 'Mr.'
GROUP BY FirstName
HAVING COUNT (firstname)>10 

Desafios : 

1- Estamos querendo identificar as provincias (stateProvinceID)com o maior numeor de cadastros no nosso sistema , então é preciso encontrar quais províncias (satateProvinceID )
estão registradas no banco de dados mais que 1000 vezes 


SELECT StateProvinceID , COUNT (stateprovinceid) AS "quantidade"
FROM person.Adress
GROUP BY StateProvinceID
HAVING COUNT (stateprovinceid)>1000

2- Sendo que se trata de uma multinacional os gerentes querem saber quais produtos (productID) não  estão trazendo em média no mínimo 1 milhão em total de vendas (linetotal)

SELECT ProductID, AVG(LineTotal)
FROM sales.SalesOrderDetail
GROUP BY ProductID
HAVING AVG(linetotal) <1000000










