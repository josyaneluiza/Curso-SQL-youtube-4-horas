Manipulaçaõ de várias palavras , caracteres.

link:https://learn.microsoft.com/pt-br/sql/t-sql/functions/string-functions-transact-sql?view=sql-server-ver16


concat : argumento  e '' para espaço entre os argumentos

SELECT CONCAT (FirstName,'',LastName)
FROM Person.Person


UPPER : TUDO MAIUSCULO 
lower : tudo minusculo 
SELECT UPPER(FirstName), 
FROM Person.Person


Len : contagem de quantos caracteres tem aquela palavra

SELECT LEN (FirstName)
FROM Person.Person


Substring: serve para estrair um pedaço dentro de uma string e numeração que indica ,abaixo  começando do indice 1 e extraindo 3 letras, como uma abreviação , por exemplo.

SELECT firstname,SUBSTRING(FirstName 1, 3)
FROM Production.Product

REPLACE : pedir para substituir algo na palavra , exemplo arco-iris , por arco#irirs, no caso substituiu - por # 

SELECT REPLACE (ProductNumber,'-','#')
FROM Production.Product

