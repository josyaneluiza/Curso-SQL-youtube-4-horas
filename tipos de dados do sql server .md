

Quatro pincipais tipos, sendo eles : 

1.Boleanos
2.Caractere
3.Números
4.Temporais

1.Boleanos 
Por padrão é inicializado como nulo, e pode receber tanto 1 ou 0
BIT
2.Caracteres 
tamanho fixo- CHAR// permite inserir até uma quantidade fixa de caracteres e sempre ocupa todo o espaço reservado 10/50 (ou seja,ele sempre ocupa 50 espaço da memoria )
Tamanho variáveis - varchar ou nvachar // permite inserir até uma quantidade que for definida, porém só usa o espaço que for preenchido 10/50 ( ou seja, vai ocupar apenas 10 , dos 50 definidos, não ocupando o restante de 40)

3.Numeros 
-Valores exatos 

1. TINYINT - não tem parte valor fracionados (ex: 1.43,24.23) somente 1,123123,324234,313123,etc...
2. Smallint - mesma coisa, porém limite maior 
3. INT - mesma coisa , porém limite maior 
4. BIGINT(maior que INT) - mesma coisa porém limite maior 
5.NUMERIC OU DECIMAL - valores exatos, porém permite ter parte fracionados, que também pode ser especificado a precisão  e a escala (escala é o número de dígitos na parte fracional) - ex: NUMERIC (5,2) 113,44

Valores Aproximados 

1. REAL - Tem precisão aproximada de até 15 dígitos 



