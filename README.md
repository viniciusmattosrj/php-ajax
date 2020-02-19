# Sobre o Projeto
Criando seus sites e sistemas utilizando o AJAX, independente se for o AJAX puro ou o usado pelo Jquery.
- <a href="https://www.asolucoesweb.com.br/curso/curso-ajax-com-php">Ajax com MVC</a> - Alexandre Cardoso


## Requerimentos

- Install <a href="https://docs.docker.com/install/">Docker</a>

- Install <a href="https://docs.docker.com/compose/install/">docker-compose</a>

- PHP >= 7.1

- Postgres >= 9.4 ou Mysql >= 5.7


## Instalação
Realizar o git clone do projeto
```bash
git clone git@github.com:viniciusmattosrj/php-ajax.git
```

Para que o git não considere alterações de permissão como modificações a serem rastreadas, execute:
```
git config core.fileMode false
```

Entre pelo terminal na pasta do projeto e rode:
```
cp ./docker-compose-example.php  ./docker-compose.php
```

Agora suba o servidor:
```
docker-compose up -d
```

Em outra aba do terminal se conecte no container do php e inicie um servidor built in do PHP
```
docker exec -it php bash
php -S 10.11.0.11:8008 -t public
```

No browser digite http://10.11.0.11:8008

Criando banco dados postgres: 

```
docker exec -it postgres bash
psql -U webadm -c "CREATE DATABASE php_ajax;"
```

Realizando a importação dump sql para a base criada:
```
psql -U webadm php_ajax < /var/lib/postgresql/sqlscript/php_ajax.sql
```

Para o acesso no <strong>POSTGRES</strong> database administration tool, use http://localhost:5050 e use as credênciais abaixo:

  - server:
  - username:
  - password:


Criando banco dados postgres: 

```
docker exec -it mysql bash
mysql -u root -c "CREATE DATABASE php_ajax;"
```

Realizando a importação dump sql para a base criada:
```
mysql -u root -p php_ajax < /var/lib/mysql57/php_ajax.sql
```

Para o acesso no <strong>MYSQL</strong> database administration tool, use http://localhost:8080 e use as credênciais abaixo:

  - server:
  - username:
  - password:


## Contribuições
Caso identifique pontos
que possam ser aprimorados envie o seu PR. ;-)


## License
[MIT](https://choosealicense.com/licenses/mit/)