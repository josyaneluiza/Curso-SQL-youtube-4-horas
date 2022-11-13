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

DESAFIO !

a equipe de produçao precisa do nome de todas as peças que pesam mais de 500 kg e nao mais de 700kg para inspeção , Peso é weight

Desafio 2 

Foi pedido a relação de todos os empregados (employees) que são casados (single= solteiro , married = casado ) e são assalariados ( salaried)

TENTEI :

SELECT *
FROM HumanResources.Employee
WHERE MaritalStatus = 'S' and SalariedFlag = '1' 