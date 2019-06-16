# Sobre o Projeto
Criando seus sites e sistemas utilizando o AJAX, independente se for o AJAX puro ou o usado pelo Jquery.
- <a href="https://www.asolucoesweb.com.br/curso/curso-ajax-com-php">Ajax com MVC</a> - Alexandre Cardoso


## Requerimentos

Install <a href="https://docs.docker.com/install/">Docker</a>

Install <a href="https://docs.docker.com/compose/install/">docker-compose</a>


## Instalação
Realizar o git clone do projeto
```bash
git clone git@github.com:viniciusmattosrj/php-ajax.git
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
php -S 10.11.0.2:8008 -t public
```

No browser digite http://10.11.0.2:8008


## Contribuições
Caso identifique pontos
que possam ser aprimorados envie o seu PR. ;-)


## License
[MIT](https://choosealicense.com/licenses/mit/)