Ordenar dados dentro de uma mesma tabela , filtrar dados dentro da tabela. 
--SELECT NOME_COLUNA
--FROM TABELA A,TABELA B
--WHERE CONDICAO
--Eu quero todos os clientes que moram na mesma regiao

SELECT A.ContactName, B.ContactName
FROM Customers A, Customers B
WHERE A.region = B.Region 

SELECT *
FROM Customers

-- Eu quero encontrar (nome e data de contrataçaõ) de todos 
--os funcionários que foram contratados no mesmo ano 

SELECT A.firstname, A.hiredate,b.firstname, b.hiredate
FROM Employees A, Employees B
WHERE DATEPART(YEAR,a.hiredate)=DATEPART(YEAR,b.HireDate)



--DESAFIO 
-- eu quero saber na tabela detalhe do pedido (order details) quais produtos
--tem o mesmo percentual de desconto

SELECT a.Discount,A.ProductID, b.discount,b.ProductID
FROM [Order Details] A, [Order Details] B
WHERE a.Discount=b.discount


