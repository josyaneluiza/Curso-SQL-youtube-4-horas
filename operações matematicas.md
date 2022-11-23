 todas as operações como 
 soma : +
 subtração: -
 multiplicação : *
 divisão : /

 exemplo : 

SELECT UnitPrice + lineTotal 
FROM Sales.SalesOrderDetail


para pegar média, por exemplo : 

SELECT AVG(LineTotal)
FROM Sales.SalesOrderDetails

pode somar; SUM
valor minimo; MIN
valor maximo; MAX

como fazer arredondamento de valores : 

Sendo o numero dois a coluna desejada( podia ser coluna 3, 4 ,etc.)

SELECT ROUND (LineTotal,2)
FROM Sales.SalesOrderDetails



Como fazer raiz quadrada de valores: 

SELECT SQRT (LineTotal)
FROM Sales.SalesOrderDetails
