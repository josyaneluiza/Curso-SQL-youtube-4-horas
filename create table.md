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

### YoutubeLite
 
 Exemplo de tabelas. Na tabela Canal o Canal ID é a primary Key e na tabela Video Canal ID e a forghet KEY . 


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











