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
DEFAULT - força um valor padrão quando nenhum valor é passado 





