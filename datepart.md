Pesquisando no google, há varias formas de executar o comando : 

Link https://learn.microsoft.com/en-us/sql/t-sql/functions/datepart-transact-sql?view=sql-server-ver16


Este comando permite selecioanr datas .

SELECT SalesOrderID, DATEPART(MONTH,OrderDate) AS MES
FROM Sales.SalesOrderHeader


PODE SE SELECIONAR TAMBÉM O DIA (DAY) E O ANO (YEAR)


SELECT AVG (TotalValue) Media, DATEPART(month, OrderDate) as Mes
FROM sales.SalesOrderHeader
GROUP BY DATEPART(year,OrderDate)
Order By Mes

Você pode colocar em ordem mensal como mostrado acima : Jnaeiro, Feveriro, março, etc ou dia ou ano , como for necessário. 


