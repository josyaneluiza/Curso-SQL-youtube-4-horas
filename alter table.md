# Como alterar a estrutura de uma tabela usando o ALTER TABLE

SINTAXE : 
ALTER TABLE nomedaTabela
ACAO

Exemplo do que pode ser feito : 

- Add, Remover, or alterar uma coluna 
- Setar valores padrões para uma coluna 
- Add ou Remover restrições de colunas 
- Renomear uma tabela 

No vídeo, ele ensina a como apagar um banco de dados  : 
botão direito ;delete; delete connection existent, delete 
E assim , ele cria outro banco de dados.


CREATE TABLE youtube (
id int primary key,
nome varchar(150) not null unique, 
categoria varchar (200) not null,
dataCriacao datetime not null
)

SELECT * from youtube


### Como adicionar uma coluna 

ALTER TABLE youtube
add ativo bit


### Como alterar o limite de 200 para 300 caracteres

ALTER TABLE youtube
ALTER COLUMN categoria varchar (300) not null


### Como alterar o nome de uma coluna, neste caso usar : 

EXEC sp_RENAME 'nomeTabela.nomeColunaAtual' , 'nomeColunaNova', 'COLUMN'

EXEC sp_RENAME 'youtube.nome' , 'nomeCanal' , 'COLUMN'

### Como alterar o nome da Tabela : 

EXEC sp_rename 'nomeTabelaAtual', 'nomeTabelaNova'

EXEC sp_rename 'youtube' , 'youtube 2' 