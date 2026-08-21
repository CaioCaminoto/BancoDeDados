-- O que foi feito para criar a base do banco de dados:

-- CREATE TABLE produtos(
--     id INT GENERATED ALWAYS AS IDENTITY NOT NULL, 
--     nome VARCHAR(50) NOT NULL,
--     preço NUMERIC(10,2) NOT NULL,
--     estoque INT NOT NULL DEFAULT 0   
-- );

--Para consultar os dados da tabela:

-- SELECT * FROM produtos;

--Para adicionar o produto, na ordem sempre:
    
INSERT INTO produtos(nome,preço,estoque)
VALUES('Chuveiro','100','20');

SELECT * FROM produtos;