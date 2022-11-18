Nós usamos o operador IN junto com o WHERE , para verificar se um valor correspondem com qualquer valor passado na lista de valores . 

valor IN (valor1,valor2)

color IN (valor1,valor2)

Valor In (SELECT valor FROM nomedaTabela)

SELECT *
FROM Person.Person
WHERE BusinessEntityID  IN (2,7,13)

PODE USAR NOT IN PARA MOSTRAR AO CONTRÁRIO TAMBÉM 
 
MAIS RÁPIDO DO QUE : 

SELECT *
FROM Person.Person
WHERE BusinessEntityID = 2
OR BusinessEntityID = 7
OR BusinessEntityID = 13
