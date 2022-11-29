# Como usar views, que são tabelas criadas para consulta onde vocÊ usa tabelas como base para criar um nova tabela de pesquisa com apenas dados específicos que você precisa de uma tabela. 

comum quando vai criar relatórios !
 

 SINTAXE : 

CREATE VIEW [Pessoas Simplificado] As
SELECT FirtName, MiddleName, LastName
FROM Person.Person 
WHERE Title = 'Ms.'

SELECT * FROM [Pessoas Simplificado]
