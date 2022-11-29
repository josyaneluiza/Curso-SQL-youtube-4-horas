# Como criar restrições de valores que podem ser inseridos em uma coluna de uma tabela em banco de dados qunado você está criando uma tabela nova 

SINTAXE : 


CREATE TABLE CarteiraMotorista(
    Id int NOT NULL, 
    Nome varchar (255) NOT NULL, 
    Idade int CHECK ( Idade >= 18)
);

SELECT * FROM CarteiraMotorista 

**INSERT INTO  CarteiraMotorista (id,nome,idade) values (1,'rafael',17)**

Neste caso acima, os dados não são inseridos na tabela por conta da restrição de idade, portanto , Rafael precisa ter 18 anos. É para isso que server o int CHECK, para ter uma restrição : 


INSERT INTO  CarteiraMotorista (id,nome,idade) values (1,'rafael',18)


Desafio : Crie 2 Tabelas novas e crie duas restrições para elas 





