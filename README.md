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

INSERT INTO (Titulo, Autor, Editora, Volume) VALUES ("Naruto","Masashi Kishimoto", "Shueisha", 43);

CREATE TABLE vendas(
ID_Vendas INT PRIMARY KEY AUTO_INCREMENT,
Quantidade INT,
VALOR DECIMAL(10,2)
);

INSERT INTO vendas (Quantidade, Valor) VALUES (35,25.50);






