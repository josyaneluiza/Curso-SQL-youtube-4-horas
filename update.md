Serve para atualizar linhas em um banco de dados :


SINTAXE

UPDATE nomeTabela
SET coluna 1 = valor1
    coluna 2 = valor2
WHERE condicao 

### É necessário colocar o WHERE , pois se não altera todo a tabela e não somente uma parte dela, gerando um grande problema. Sem o where : 

UPDATE Aula
SET nome = 'teste'


SELECT *  FROM Aula


|id|nome|
|--|----|
|1|teste|
|2|teste|
|3|teste|
|4|teste|

### Com o Where : 

UPDATE Aula
SET nome = 'mudei'
WHERE id = 3


|id|nome|
|--|----|
|1|teste|
|2|teste|
|3|mudei|
|4|teste|


SELECT *  FROM Aula