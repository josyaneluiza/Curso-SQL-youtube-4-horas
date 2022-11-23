O operador union combina dois ou mais resultados de um select em um resultado apenas . 

SELECT coluna1, coluna2
FROM tabela1
UNION
SELECT coluna1, coluna2 
FROM tabela2

union remove os resultados duplicados

UNION ALL junta até os resultados duplicados 

Você pode até usar order by desc para arrumar as tabelas

EXEMPLO 2 : 
SELECT FirstName, Title
FROM person,person 
WHERE Title = 'Mr.'
UNION 
SELECT FirstName, Title , MiddleName
FROM Person.person 
WHERE MiddleName= 'A' 

