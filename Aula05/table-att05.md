-- -- CREATE TABLE catalogo( 
-- -- id INT GENERATED ALWAYS AS IDENTITY NOT NULL, 
-- -- nome VARCHAR(50) NOT NULL,
-- -- duracao INT NOT NULL,
-- -- avaliacao NUMERIC(3,1) NOT NULL
-- -- );

-- SELECT * FROM catalogo;

-- INSERT INTO catalogo(nome,duracao,avaliacao)
-- VALUES ('Corações de Ferro', 134, 7.6),
-- ('Deadpool & Wolverine',134 ,7.5),
-- (' O Lobo de Wall Street ',180 ,8.2),
-- (' Riphagen: O Intocável',131 ,7.1),
-- ('Nada de Novo no Front ',147 ,7.8),
-- ('Interstellar',169 ,8.7),
-- ('Vingadores: Ultimato',181 ,8.2),
-- ('Oppenheimer',180 ,8.0),
-- ('Um Filme Minecraft',101 ,5.6),
-- ('Backrooms',110 ,6.4),
-- ('O Resgate do Soldado Ryan',169 ,8.6),
-- ('Até o Último Homem',139 ,8.1),
-- ('Breaking Bead',3.038 ,9.5),
-- ('Dexter',5.088 ,8.6),
-- ('Better Call Saul',3.150 ,9.0),
-- ('O Mentalista',6.493 ,8.2),
-- ('Black Mirror',2.040 ,8.7),
-- ('Pluribus',486 ,7.7),
-- ('Love, Death & Robots',525 ,8.4),
-- ('Avatar: A Lenda de Aang',3.600 ,9.3),
-- ('Naruto',5.280 ,8.4);

-- -- DELETE FROM catalogo 
-- -- WHERE id=1

-- SELECT * FROM catalogo
-- ORDER BY avaliacao DESC
-- LIMIT 10;

-- UPDATE catalogo
-- SET avaliacao=10
-- WHERE id IN (1,2,3,4,5);

-- DELETE FROM catalogo
-- WHERE id IN (1,2,3,4,5);