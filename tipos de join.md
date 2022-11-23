|A|          |  B|
|---|        |----|
|id nome|    |id nome|
|------|     |------|
|1 Robo|     |1 Espada |
|2 Macaco |   |2 Robo|
|3 Samurai|   |3 Mario|
|4   Monitor|  |4 Samurai|


 Registros iguais : Robo e Samurai.
 Registros nãi iguais : Macaco, Espada, Mario, Monitor. 

 * Inner Join :

 Inner Join retorna apenas os resultados que correspondem (existem) tanto na tabela A como Tabela B (registros iguais).

 SELECT * FROM TabelaA 
 INNER JOIN TabelaB
 ON TabelaA.nome = TabelaB.nome

 Retorna sempre a interseção (noção de conjuntos)

Full Outer Join 
Full outer join retorna um conjunto de todos registros correspondentes da TabelaA e TabelaB quando são iguais. E ,além disso, se não houver valores correspondentes, ele simplesmente irá preencher esse lado ''null'' (join que vai incluir mais informação).

SELECT * 
FROM Tabela A 
FULL OUTER JOIN Tabela B
ON TabelaA.nome = TabelaB.nome

tudo o que existe em comum e tudo o que tem de diferente em um conjunto só.

 * LEFT OUTER JOIN
Left outer join um conjunto de todos os registros da TabelaA, e além disso, os registros correspondentes (quando disponívies) na TabelaB. Se não houver registros correspondentes ele simplismente vai preencher com "null"

somente conjunto a e interseção com B, excluindo o conjunto b que tem itens que não são repetidos

SELECT *
FROM TabelaA
LEFT JOIN TabelaB
ON TabelaA.nome = TabelaB.nome






