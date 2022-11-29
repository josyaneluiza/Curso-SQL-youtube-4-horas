# Como dropar (excluir) uma tabela do banco de dados, usando o DROP TABLE

SINTAXE 

DROP TABLE nomeDaTabela

### TABELAS QUE SÃO REFERENCIADAS NÃO PODEM SER APAGADAS  :

DROP table person.Address (NÃO É POSSÍVEL APAGAR)

DROP table ErrorLog (É possível apagar)


### Como apagar os dados de uma tabela sem apagar a tabela ( apenas esvaziar seu conteúdo )


TRUNCATE TABLE Person.password