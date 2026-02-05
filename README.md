# loja_livros
Estudo de criação de tabela em SQL baseado em uma loja fictícia de livros e mangás.
CREATE DATABASE loja_livros;

CREATE TABLE produtos

(ID_Produto INT PRIMARY KEY AUTO_INCREMENT,
Titulo VARCHAR(150),
Autor VARCHAR(100),
Editora VARCHAR(100),
Volume INT);

CREATE TABLE vendas(
ID_Vendas INT PRIMARY KEY AUTO_INCREMENT,
Quantidade INT,
VALOR DECIMAL);






