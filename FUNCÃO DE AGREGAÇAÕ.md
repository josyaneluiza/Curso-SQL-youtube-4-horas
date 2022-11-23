Função de agregação MIN MAX SUM AVG 

funções de agregação basicamente agregam ou combinam dados de uma tabela em 1 resultado só


COmo somar todas as vendas :
ELECT TOP 10 sum(lineTotal) AS "SOMA"
FROM Sales.SalesOrderDetail

Mínimo ou máximo de vendas:
SELECT TOP 10 MIN(lineTotal) AS "SOMA"
FROM Sales.SalesOrderDetail

Média de vendas:

SELECT TOP 10 AVG(lineTotal) AS "SOMA"
FROM Sales.SalesOrderDetail
