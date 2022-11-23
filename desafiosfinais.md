1-Quantos produtos temos cadastrado no sistema que custam mais que 1500 dolares 

SELECT COUNT (listprice)
FROM Production.Product 
WHERE listprice > 1500

2- Quantas pessoas temos com o sobrenome que  inicia com a letra P

SELECT COUNT (lastname)
FROM person.Person 
WHERE Lastname like 'p%'

3-Em quantas cidades únicas estão cadastrados nossos clientes?

SELECT COUNT(DISTINCT(city) 
FROM person.Address

4-Quais são as cidades únicas que temos cadastradas em nosso sistema?

SELECT DISTINCT(city)
FROM person.Address

Quantos produtos tem a cor vermelha com preço entre 500 e 1000 dolares                                      

SELECT COUNT(*)
FROM Production.Product
Where color = 'red' and ListPrice BETWEEN 500 AND 1000

6-
Quantos produtos cadastrados tem a palavra 'road' no nome deles?

SELECT COUNT(*)
FROM Production.Product
WHERE name like '%road%'





