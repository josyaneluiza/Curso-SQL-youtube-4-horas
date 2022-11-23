SELECT dentro do select, um query mais poderoso e compleox 

--Monte um relatório de todos os produtos cadastrados que tem preço de venda acima de média

-- Primeira coisa é descobrir onde eles estão .


SELECT  AVG(ListPrice)
FROM Production.Product


SELECT *
FROM Production.Product
WHERE ListPrice > 438.66

SELECT *
FROM Production.Product
WHERE ListPrice >

--USANDO O SUBSELECT PARA FACILITAR A PESQUISA :

SELECT *
FROM Production.Product
WHERE ListPrice > (SELECT AVG(ListPrice) FROM Production.Product
