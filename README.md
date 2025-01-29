# sql-desafio-gestao-biblioteca

create table livros (
id int not null auto_increment primary key,
titulo varchar(100) not null,
autor varchar(100) not null,
ano_publicacao int not null,
genero varchar(50) 
 );
 
insert into livros (titulo, autor, ano_publicacao, genero) values 
 ("1984", "George Orwell", 1949, "Ficção Distópica"),
 ("Dom Quixote", "Miguel de Cervantes", 1605, "Romance"),
 ("Cem Anos de Solidão", "Gabriel García Márquez", 1967, "Realismo Mágico");
 
 alter table livros add column editora varchar(100) not null after ano_publicacao;
 
update livros set editora = "Companhia das Letras" where id = 1;
update livros set editora = "Editora 34" where id = 2;
update livros set editora = "Record" where id = 3;

select * from livros where ano_publicacao > 1900;
select * from livros where genero = "Romance";
select id from livros;
select count(*) from livros;
 
 select * from livros;
 
