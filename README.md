# Boas vindas ao repositório backend do projeto de Deploy - Stranger Things!

Aqui você vai encontrar os locais para colocar suas repostas relativas aos requisitos de backend.

**Lembre-se**: coloque as respostas apenas dos requisitos que contém o seguinte direcionamento:

  - Adicione os comandos utilizados, de maneira sequencial, ao README do backend.

**Nota**: Este direcionamento está presente no [repositório](https://github.com/tryber/sd-01-block31-stranger-things) em que os requisitos do projeto são destrinchados.

## Requisitos

### 6 - Deploy Heroku

Para realizar o deploy do meu backend, fiz o seguinte procedimento:

`heroku create --remote hawkings deploy-backend-hawkings-doug-1224`

`heroku create --remote upside-down deploy-backend-upsidedown-doug-1224`

`heroku config:set TRYBE="false" --app deploy-backend-hawkings-doug-1224`

`heroku config:set TRYBE="true" --app deploy-backend-upsidedown-doug-1224`

`git add` .

`git commit -m "Iniciando deploy no projeto backend"`

`git push hawkings doug-funny-stranger-things-backend:master`

`git push upside-down doug-funny-stranger-things-backend:master`

### 7 - Monitoramento

Para conseguir realizar o monitoramento da minha API, fiz o seguinte procedimento:

`heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA_AQUI" PM2_SECRET_KEY="CHAVE_PRIVADA_AQUI" --app deploy-backend-hawkings-doug-1224`

`heroku config:set PM2_MACHINE_NAME=heroku-server --app deploy-backend-hawkings-doug-1224`

`heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA_AQUI" PM2_SECRET_KEY="CHAVE_PRIVADA_AQUI" --app deploy-backend-upsidedown-doug-1224`

`heroku config:set PM2_MACHINE_NAME=heroku-server --app deploy-backend-upsidedown-doug-1224`
