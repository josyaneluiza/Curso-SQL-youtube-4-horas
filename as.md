Serve basicamente para renomear uma coluna , bem simples . 


exemplo : SELECT TOP 10 ListPrice as "preço do produto"
FROM Production.Product
 

1 ) encontrar o FirstName and Last Name e renomear em portugues 

2 )ProductNumber renomear para Numero do produto da tabela prodution.product

3) sales.SalesOrderDetail unitPrice "Preço único "


SELECT FirstName as "primeiro nome", LastName as "Segundo nome"
FROM Person.Person


SELECT ProductNumber as "Numero do Produto"
FROM Production.Product


SELECT UnitPrice AS "Preço Unitário"
FROM Sales.SalesOrderDetail
