## ATIVIDADE BANCO DE DADOS STREAMING

1- Primeiro entramos no postgresql.
![alt text](image.png)

2-Após entramos no postgres criamos o nosso banco de dados do streaming
![alt text](<Captura de tela 2026-08-21 100455.png>)

e vemos se ele realmente foi criado certinho usando o comando "l".

![alt text](<Captura de tela 2026-08-21 100504.png>)

3- Agora entramos no VsCode e na extensao PostgreSQL explorer, aonde reentramos usando nosso ip e damos um refresh para aparecer o "betaflix".

4-Já na extensão damos o comando CREATE TABLE para criar a base do banco de dados o catalogo aonde vão ficar as informações do filme

![alt text](<Captura de tela 2026-08-21 102348.png>)

comentamos o código passado, e já verificamos se tudo ficou como queriamos apertando f5 e usando o comando SELECT.

![alt text](<Captura de tela 2026-08-21 102406.png>)

5-Agora preenchemos a tabela usando o INSERT INTO, colocando 21 filmes e séries
![alt text](<Captura de tela 2026-08-21 105311.png>)

e verificamos novamente 
![alt text](<Captura de tela 2026-08-21 105315.png>)

vemos que o Corações de Ferro se repetiu e o apagamos pelo id para ficar só um dele
![alt text](<Captura de tela 2026-08-21 105903.png>)

e vemos que realmente deu certo
![alt text](<Captura de tela 2026-08-21 110937.png>)

5- Agora para vermos os 10 melhores filmes e séries usamos o SELECT * FROM e só filtramos as maiores notas e os 10 melhores
![alt text](<Captura de tela 2026-08-21 111316.png>)

e como podemos ver realmente deu certo e retornou os 10 melhores.
![alt text](<Captura de tela 2026-08-21 111323.png>)

6- Agora alteramos a nota de alguns deles para 10, do id 1 ao 5 utilizamos o IN para facilitar nossa vida e não precisar colocar vários OR 
![alt text](<Captura de tela 2026-08-21 112038.png>)

e agora vemos que do id 1 ao 5 realmente todos estão com nota 10.

![alt text](<Captura de tela 2026-08-21 112058.png>)

7- Agora apagaremos do id 1 ao 5 
![alt text](<Captura de tela 2026-08-21 112510.png>)

E vemos que agora os filmes começam no id 6 por termos apagado até o 5.

![alt text](<Captura de tela 2026-08-21 112526.png>)

*e essa foi atividade STEAMING da aula/semana 5*
