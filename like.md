Vamos dizer que você quer encontrar uma pessoa no banco de dados em que o nome dela era ovi.. alguma coisa 


SELECT *
FROM person.person
WHERE FirstName like 'ovi%' 

( inicio do nome)

ovini

para final do nome 
(%to)

augusto

para o meio do nome 
(%essa%)
 vanessa

não lembrava a proxima letra
 (%ro_)
 Aaron 

 independente deo maiusculo ou minusculo o resultado é sempre o mesmo 

(%RO), (%Ro), etc



