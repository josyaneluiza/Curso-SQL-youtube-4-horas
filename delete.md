Altereção e remoção do banco de dados : Apagar linhas 

SINTAXE 

DELETE FROM nomeTabela
WHERE condicao 

### é importante colocar o WHERE para não apagar tudo! 

DELETE FROM Aula
WHERE nome = 'mudei'

SELECT * FROM Aula

Ficando : 

|id|nome|
|--|----|
|1|teste|
|2|teste|
|4|teste|

Sem selecionar o WHERE,  as linhas 1, 2, e 4 também apagariam !