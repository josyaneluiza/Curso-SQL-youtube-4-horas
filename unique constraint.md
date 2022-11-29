Como ter colunas únicas, porém diferente de uma primary key , pode existir várias colunas com a restrição UNIQUE . Permite não inserir dados repetidos. 

CREATE TABLE CarteiraMotorista(
    Id int NOT NULL, 
    Nome varchar (255) NOT NULL, 
    Idade int CHECK ( Idade >= 18),
    CodigoCNH int NOT NULL UNIQUE
);


insert into CarteiraMotorista( Id,Nome,Idade,CodigoCNH) values (1,'robert',19,123456)
 
 **Consigo iserir , porém se eu repitir não é possivel inserir campos repetidos**

 insert into CarteiraMotorista( Id,Nome,Idade,CodigoCNH) values (1,'robert',19,123456)
 




