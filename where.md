SELECT coluna1,coluna2,coluna3,coluna4
FROM tabela
WHERE condição

/*

|OPERADOR|DESCRIÇÃO
|--------|---------|
|=|IGUAL|
|>|MAIOR QUE|
|<|MENOR QUE|
|>=|MAIOR QUE OU IGUAL|
|<=|MENOR QUE OU IGUAL|
|<>|DIFERENTE DE |
|AND| OPERADOR LOGICO|
|OR|OPERADOR LOGICO OU|

DESAFIO 1

a equipe de produçao precisa do nome de todas as peças que pesam mais de 500 kg e nao mais de 700kg para inspeção , Peso é weight

SELECT Name
FROM production.produtc
WHERE weight <500 and weight >700

Desafio 2 

Foi pedido a relação de todos os empregados (employees) que são casados (single= solteiro , married = casado ) e são assalariados ( salaried)

TENTEI :

SELECT *
FROM HumanResources.Employee
WHERE MaritalStatus = 'M' and SalariedFlag = '1' 

Acertei ! 

Desafio 3 


SELECT * 
FROM Person.Person
WHERE FirtsName = 'peter' and LastName = 'krebs'

SELECT * 
FROM PERSON.EmailAdress
WHERE BusinessEnityID = '26'

