# loja_livros
Estudo de criação de tabela em SQL baseado em uma loja fictícia de livros e mangás.
CREATE DATABASE loja_livros;

CREATE TABLE produtos
(ID_Cliente INTEGER PRIMARY KEY AUTO_INCREMENT,
Titulo TEXT, 
Autor TEXT, 
Editora TEXT, 
Volume INTEGER);

INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("Naruto","Masashi Kishimoto","Shueisha", 15);
INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("Boku No Hero", "Kohei Horikoshi", "Shueisha",20);
INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("Monster", "Naoki Urasawa","Shogakukan",12);
INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("Gachiacuta", "Hiroshi Seko", "Kodansha",16);
INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("Jujutsu Kaisen", "Gege Akutami", "Shueisha",22);
INSERT INTO produtos(Titulo, Autor, Editora, Volume) VALUES ("One Piece", "Eiichiro Oda", "Shueisha",45);
            
CREATE TABLE vendas

(ID_Cliente INTEGER PRIMARY KEY AUTO_INCREMENT, 
Quantidade INTEGER,
Valor INTEGER);

INSERT INTO vendas (Quantidade, Valor) VALUES (50,23.50);
INSERT INTO vendas (Quantidade, Valor) VALUES (38,15.99);
INSERT INTO vendas (Quantidade, Valor) VALUES (35,24.50);
INSERT INTO vendas (Quantidade, Valor) VALUES (60,30.00);
INSERT INTO vendas (Quantidade, Valor) VALUES (72,20.00);
INSERT INTO vendas (Quantidade, Valor) VALUES (68,35.00);




