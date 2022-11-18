Serve para juntar informações diferentes de outras tabelas


Existem 3 tipos de join : 

INNER JOIN, OUTER JOIN, SELF-JOIN


INNER JOIN : 

EXPLICANDO : 


|CLIENTE|
|------|
|CLIENTELD|
|NOME|
|ENDERECOLD|  


|ENDEREÇO|
|-------|
|ENDERECOLD|
|RUA|
|CIDADE| 

VAMOS DIZER QUE TEMOS ESSAS DUAS TABELAS ,vamos dizer que vocÊ queria trazer informação para a tabela cliente, no caso endereço, nesse caso temos que fazer um join . 

Nos temos que pegar o ID do cliente e os outros dados, pois o enderecold é uma chave estrangeira, fazendo um ligaçaõ entre eles. 


COMO ? 

SELECT C.ClienteID , C.Nome, E.Rua, E.Cidade
FROM Cliente C
INNER JOIN Endereço E on E.EndereçoID = C.EndereçoID

Sendo um resultado como ,por exemplo : 

|Cliente|
|------|
|2 |
|Bruno|
|Rua Norte|
|São Paulo |





Juntar: 

--BusinessEntityID, FirstName,LastName,EmailAdresss


SELECT TOP 10 *
FROM Person.Person


SELECT TOP 10 *
FROM Person.EmailAddress

Coluna em comum BusinessEntityID 

SELECT p.BusinessEntityID,FirstName,LastName,EmailAddress (colunas da 1 tabela)
FROM Person.Person as P
INNER JOIN Person.EmailAddress PE on p.BusinessEntityID = pe.BusinessEntityID (informações da segunda tabela + colunas em comum )


Exemplo 2 : 
Vamos dizer que nós queremos os nomes dos produtos e as informações de suas subcategorias

---ListPrice,Nome do produto, Nome da Subcategoria 

SELECT pr.ListPrice, pr.Name,pc.Nmae
FROM Production.Product Pr
INNER JOIN Production.ProductSubcategory PC on PC.ProductSubcategoryID = pr.ProductSubcategoryID


-Juntar tudo das tabelas / Produto cartesiano :

SELECT TOP 10 *
FROM Person.BusinessEntityAddress

SELECT TOP 10 *
FROM Person.Address


SELECT TOP 10 * <----Usar o asterisco para selecionar tudo 
FROM Person.PersonEntityAddress BA
INNER JOIN Person.Address PA on PA.AddressID = BA.AddressID



Desafio 1 : 

SELECT TOP 10 *
FROM Person.PhoneNumberType

SELECT TOP 10 *
FROM Person.PersonPhone

SELECT pp.BusinessEntityId, pt.name, pt.PhoneNumberTypeID,pp.PhoneNumber
FROM person.PersonPhone PP
INNER JOIN Person.PhoneNumberType PT ON PT.PhoneNumberTypeID = pp.PhoneNumberTypeID


Desafio 2 : 

--AddressID , City, StateProvindeID , Nome do Stado 

SELECT TOP 10 * 
FROM person.stateprovince


SELECT TOP 10 PA.AddressID, PA.City, PS.StateProvinceID, PS.Name 
FROM person.address PA
INNER JOIN Person.StateProvince PS ON PS.StateProvinceID = PA.StateProvinceID 




