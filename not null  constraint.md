  
  # Como criar restrições forçam com que não seja possível inserir dados em uma tabela sem preencher a coluna marcada como NOT NULL

  SINTAXE : 

  CREATE TABLE CarteiraMotorista(
    Id int NOT NULL, 
    Nome varchar (255) NOT NULL, 
    Idade int CHECK ( Idade >= 18)
)

insert into CarteiraMotorista (Id,Nome,Idade) values (1,,19)

O comando acima não foi inserido na tabela, visto que o espaço entre as vígulas indica que nada foi inserido, ficando nulo . A restrição not null indica que o campo não pode ficar nulo, não adicionando nenhuma informação ,quando solicitado , sem o campo ter algo e não ser nulo, não permite valores vazios. 

insert into CarteiraMotorista (Id,Nome,Idade) values (1,'Jhonathan',19)



