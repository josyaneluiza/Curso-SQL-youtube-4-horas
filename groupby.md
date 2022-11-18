 - O group by basicamente divide o resultado da sua pesquisa em grupos 
 - Para cada grupo que vocÊ aplicar uma função de agregaçaõ, por exemplo :
 -calcular a soma de itens 
 - contar o número de itens naquele grupo 


 SELECT coluna1, funcaoAgregacao (coluna2)
 FROM nomeTabela
 GROUP BY coluna1

Este comando soma : 
Quantas Josyanes tem no banco de dados 
Quantos são jovens 
Quantos produtos vendidos 
ETC... 
ELE SOMA AS QUANTIDADES, FORMA GRUPOS ESPECÍFICOS

SÃO USADOS AS FUNÇÕES DE AGREGAÇÃO E TAMBÉM PODE USAR O COMANDO COUNT 

 SELECT *
FROM Sales.SalesOrderDetail

SELECT SpecialOfferID, SUM (unitPrice) AS "SOMA"
FROM Sales.SalesOrderDetail
GROUP BY SpecialOfferID


SELECT color, AVG (listprice) "preco"
FROM Production.Product
WHERE Color = ' Silver'
GROUP BY Color 

Desafios : 

Preciso saber quantas pessoas tem o mesmo MiddleName agrupadas por o MiddleName 

SELECT MidlleName , COUNT  (firstname)
FROM Person.Person 
Group BY MiddleName 

2- Eu preciso saber em média qual é a quantidade (quantity) que cada produto é vendido na loja 

SELECT ProductID , AVG(OrderQty) "media"
FROM Sales.SalesOrderDetail
GROUP BY ProductID


3- Eu quero saber quais foram as 10 vendas que no total tiveram os maiores valores de venda ( linetotal )por produto do maior valor para o menor 

SELECT TOP 10 productid, SUM (linetotal)
FROM Sales.SalesOrderDetail
GROUP BY productid
ORDER BY SUM(linetotal) DESC

4- Eu preciso saber quantos produtos e qual e quantidade media de produtos temos cadastrados nas nossas ordem de serviços (WorkOrder), agrupadas por produtID 


SELECT productid, COUNT (productid) "contagem", 
AVG (orderqty)as "media"
FROM Production.WorkOrder
GROUP BY ProductID


