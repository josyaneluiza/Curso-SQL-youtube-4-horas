Quero descobrir quais pessoas tem um cartão de crédito registrado

SELECT * 
FROM Person.Person PP 
LEFT JOIN Sales.PersonCreditCard PC 
ON PP.BusinessEntityID = PC.BusinessEntityID 
WHERE PC.BusinessEntityID IS NULL <----- ( descobre  quem não tem cartão )

Usando o inner join : 19118-19972 = 854 descobre quantas pessoas tem um cartão de crédito . 

Union : 
