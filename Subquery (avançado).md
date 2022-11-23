SELECT dentro do select, um query mais poderoso e compleox 

--Monte um relatório de todos os produtos cadastrados que tem preço de venda acima de média

-- Primeira coisa é descobrir onde eles estão .


SELECT  AVG(ListPrice)
FROM Production.Product


SELECT *
FROM Production.Product
WHERE ListPrice > 438.66


--USANDO O SUBSELECT(subquery)
 PARA FACILITAR A PESQUISA :

SELECT *
FROM Production.Product
WHERE ListPrice > (SELECT AVG(ListPrice) FROM Production.Product

 Eu quero saber o nome dos meus funcionários que tem o cargo desing enginneer. 


 SELECT*
 FROM person.Person 
 ( NÃO Vamos fazer baseado no BusinessEntityID, POIS  ele só seelecionaria alguns
 )

 SELECT *
 FROM HumamResources.Employee
 WHERE JobTitle = 'Desing Engineer 
 
Usando o suqquery


SELECT FirstName
FROM Person.Person 
WHERE BussinessEntityID IN (
    SELECT BusinessEntityID 
    FROM HumanResources.Employeee
    WHERE JobTitle = 'Desing Engineer'
)

SELECT FirstName
FROM Person.Person P
INNER JOIN HumanResources.Employee E ON P.BusinessEntityID = E.BusineesEntity  
AND E.JobTitle = 'Desing Engineer' 

