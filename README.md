# Projeto Rotten Potatoes Microsserviços

## Estrutura do projeto
Esse projeto é baseado em uma aquitetura de Microsserviços e depende de outros 2 projetos pra funcionar


- [Serviço de Filmes](https://github.com/daniel10-souza/movie)
- [Serviço de Review](https://github.com/daniel10-souza/review)

Segue abaixo o diagrama:

![Diagrama da solução](./img/diagrama.png)

## Configuração

MOVIE_SERVICE_URI => URL de acesso ao serviço de listagem de filmes

REVIEW_SERVICE_URI => URL de acesso ao serviço de listagem de reviews

Exemplo:

MOVIE_SERVICE_URI: http://movies:8181

REVIEW_SERVICE_URI: http://review:8282

## Alterações

Arquivo app.py foi alterado na ultima linha: return send_file('static/' + str(path))
