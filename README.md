# loja_livros
Estudo de criação de tabela em SQL baseado em uma loja fictícia de livros e mangás.

-- Criação de um livraria fictícia -- 

CREATE DATABASE livrariafic;
-- --
USE livrariafic;


CREATE TABLE produtos
( 
id_produto INT PRIMARY KEY AUTO_INCREMENT,
Titulo VARCHAR(150) NOT NULL,
Editora VARCHAR(150) NOT NULL,
Autor VARCHAR (100) NOT NULL,
Volume INT NOT NULL,
Ano INT NOT NULL
);



INSERT INTO produtos (Titulo, Editora, Autor, Volume, Ano) VALUES ("Naruto","Shueisha", "Masashi Kishimoto",43,2010);
INSERT INTO produtos (Titulo, Editora, Autor, Volume, Ano) VALUES ("Harry Potter e a Pedra Filosofal","Rocco", "JK Rowlling",01,1997);
INSERT INTO produtos (Titulo, Editora, Autor, Volume, Ano) VALUES ("My Hero Academy","Shueisha", "Kohei Horikoshi",20,2018);
INSERT INTO produtos (Titulo, Editora, Autor, Volume, Ano) VALUES ("Silencio dos Inocentes","Record", "Thoma Harris",01,1988);
INSERT INTO produtos (Titulo, Editora, Autor, Volume, Ano) VALUES ("Introdução à Linguagem SQL","Novatec", "Thomas Nield",01,2016);


CREATE TABLE vendas
(
id_venda INT PRIMARY KEY AUTO_INCREMENT,
id_produto INT NOT NULL,
id_cliente INT NOT NULL ,
Quantidade INT NOT NULL,
valor_unitario DECIMAL(10,2) NOT NULL,
Data_venda DATE NOT NULL,

FOREIGN KEY (id_produto) REFERENCES produtos(id_produto)
)
AUTO_INCREMENT = 100;

INSERT INTO vendas (id_produto, id_cliente, Quantidade, valor_unitario, Data_venda) VALUES (2,260,3,25.00,'2026-02-10');
INSERT INTO vendas (id_produto, id_cliente, Quantidade, valor_unitario, Data_venda) VALUES (1,261,3,27.00,'2026-01-25');
INSERT INTO vendas (id_produto, id_cliente, Quantidade, valor_unitario, Data_venda) VALUES (3,262,5,22.00,'2026-01-14');
INSERT INTO vendas (id_produto, id_cliente, Quantidade, valor_unitario, Data_venda) VALUES (4,263,2,45.00,'2026-02-01');
INSERT INTO vendas (id_produto, id_cliente, Quantidade, valor_unitario, Data_venda) VALUES (5,264,1,32.00,'2026-02-03');











