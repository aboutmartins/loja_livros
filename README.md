# loja_livros
Estudo de criação de tabela em SQL baseado em uma loja fictícia de livros e mangás.
CREATE DATABASE loja_livros;

CREATE TABLE produtos

(ID_Produto INT PRIMARY KEY AUTO_INCREMENT,
Titulo VARCHAR(150),
Autor VARCHAR(100),
Editora VARCHAR(100),
Volume INT
);

INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("Naruto","Masashi Kishimoto", "Shueisha", 43);
INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("Harry Potter e a Pedra Filosofal","JK Rowling", "Rocco", 01);
INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("My Hero Academy","Kohei Horikoshi", "Shueisha", 20);
INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("Monster","Naoki Urasawa", "Shogakukan", 15);
INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("Silêncio dos Inocentes","Thomas Harris", "Record", 01);
INSERT INTO produtos (Titulo, Autor, Editora, Volume) VALUES ("Introdução à Linguagem SQL","Thomas Nield", "Novatec", 01);








