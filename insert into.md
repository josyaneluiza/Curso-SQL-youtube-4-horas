Insert INTO nomeTabela (coluna1,coluna 2,...)
VALUES (valor1,valor2)



2.Caso queira inserir várias linhas: 

Insert INTO nomeTabela (coluna1,coluna 2,...)
VALUES (valor1,valor2)
VALUES (valor1,valor2)
VALUES (valor1,valor2)
VALUES (valor1,valor2)


3.Inserir informações de uma tabela dentro de uma tabela existente : 

INSERT INTO TabelaA (coluna1)
SELECT coluna2
FROM tabelaB


No Banco de dados : 

CREATE TABLE Aula (
id int primary key,
nome varchar(200),
);

SELECT * FROM Aula

INSERT INTO Aula(id,nome)
VALUES (1,'aula 1')


--Inserir varias linhas ao mesmo tempo : 

INSERT INTO Aula (id,nome)
VALUES 
(2,'Aula 2'),
(3,'Aula 3'),
(4,'Aula 4');

--Copiar os dados de uma tabela para outra: como cirar uma rapidamente 

SELECT * INTO tabelaNova FROM Aula

Select * FROM tabelaNova



as tabelas Aula e TabelaNova aparecem da seguinte maneira quando selecionado F5 : 

|AULA|
|id|nome|
|---|---|
|1|Aula 1|
|2|Aula 2|
|3|Aula 3|
|4|Aula 4|


Desafio: 

1.Crie uma tabela nova
2.Insira um linha de dados nela
3.Insira 3 linhas de dados ao mesmo tempo 
4.Crie uma segunda tabela 
5.Insira 1 linha nessa tabela nova
6.Copie os dados da segunda tabela para a primeira . 