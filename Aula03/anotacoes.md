## Configurando o SGBD 
SGBD: Sistema Gerenciador do Banco de Dados
Para instalação, utilizamos o comando

```bash
sudo apt install -y postgresl
```
>No meu sevidor, como eu já estava como root, não foi necessário o uso do sudo.

Para acesso inicial utilizamos o comando 
```bash
sudo -u postgres psql
```
>Autenticação via linux, não necessita de senha, pois você já está autenticado 

após o primeiro acesso. alteramos a senha, através do comando: 
 ```bash
 ALTER USER postgres PASSWORD `1234´
 ```
 Para sair do SGBD, utilizamos o comando 
 ```bash 
  \q
```
 Para acesso externo, utilizamos o comando: 
 ```bash
 sudo psql -h 127.0.1 -U postgres 
 ```

 >Aqui, ele vai necessitar de senha! 

Alteração nos arquivos:
1. Navegamos até o arquivo postgres, usando cd e ls para se mover e conferir os arquivos disponiveis.

```bash
cd /etc/postgresql/18/main 
```

![alt text](<print 01-2.png>)

2. Editamos o arquivo postgresql.conf através do comando:

```bash
sudo nano postgresql.conf
```

![alt text](<print 02-1.png>)

3. Aqui alteramos o arquivo pg_hba.conf:
```bash
sudo nano ph_hba.config
```

![alt text](<print 03-1.png>)

> 3.1- Aqui acima, modificamos as duas ultimas linhas. Na linha de cima colocamos nosso ip modificado mas com o zero no final por ser neutro e "/24 por ele liberar todas as faixas de ip fazendo com que todos conseguigam logar no postgresql.

> 3.2- Na ultima linha do arquivo realizamos a mesma coisa mas agora colocando o ip como "0.0.0.0"  por ser neutro ele vai fazer com que qualquer um com a senha consiga acessar de qualquer lugar do mundo e novamente o "/24".

4. Agora começaremos a criar nosso primeiro banco de dados.
Usamos o comando a baixo para ver os banco de dados:
```bash
\l
```
![alt text](<print 04-1.png>)
e "espaço + q" para sair

e agora para criarmos o nosso primeiro banco de dados, utilizamos:

```bash
CREATE DATABASE cidade;
```
Cidade sendo o nome do nosso banco, verificamos se está lá usando "\l" e como podemos ver na imagem passada está.

5. Devido as modificações que fizemos reiniciamos o postgresql para ter certeza que deu certo:

```bash
sudo systemctl restart postgresql
```
e para ver se está tudo certo e com ele ligado usamos:

```bash
sudo systemctl status postgresql 
```

![alt text](<print 05-1.png>)

e aqui vemos que ele esta "active" então tudo certo.