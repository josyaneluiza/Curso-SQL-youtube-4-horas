Como criar uma tabela ? 

SINTAXE :


CREATE TABLE nomeTabela (
    coluna1 tipo restricaoDaColuna,
    coluna2 tipo restricaoDaColuna,
    coluna3 tipo restricaoDaColuna, 
    ...
)

Pode houver ocasiões onde não haverá restrições 


 ## Principais tipos de restrições que podem ser aplicadas 

NOT  NULL - não permite nulos
UNIQUE - Força que todos os valores em uma coluna sejam diferentes
PRIMARY KEY - uma junção de NOT NULL E UNIQUE 
FOREIGN KEY - identifica únicamente uma linha em outra tabela 
CHECK - FORÇA uma condição específica em uma coluna 
DEFAULT - força um valor **padrão** quando nenhum valor é passado 

### Youtube Lite
 
 Exemplo de tabelas. Na tabela Canal o Canal ID é a primary Key e na tabela Video  o Canal ID e a forghet KEY . 


|canal|
|-----|
|+ canalld     intPK|
|+Nome varchar(150)  not null|
|+Contagemincritos    intdefault 0|
|+DataCriacao datetime not null|


|video|
|----|
|+Videold     int Pk|
|+Nome varchar(150)   not null|
|+Vizualizaçoes      int default 0|
|+Likes        int default 0 |
|+Dislikes     int default 0 |
|+duracao     int not null|
|+Canalld   FK|



Criando no SQL : 

Create new table , name Youtube, 

New Query 

CREATE TABLE Canal (
CanalID int PRIMARY KEY, 
Nome VARCHAR (150) NOT NULL,
ContagemInscritos INT DEFAULT 0, 
DataCriaçao DATEtime not null
);

CREATE TABLE  Video (
VideoID INT PRIMARY KEY ,
Nome VARCHAR (150) NOT NULL,
Vizualizacoes INT DEFAULT 0,
LIKES INT DEFAULT 0,
Dislikes INT default 0,
Duraçao INT NOT NULL, 
CanalID INT FOREIGN KEY REFERENCES Canal(CanalID)
);

Desafio : Encontrar duas coisas na sua casa que podem se tornar tabelas e criar duas tabelas que tem no mínimo 1 relacionamento com a outra











