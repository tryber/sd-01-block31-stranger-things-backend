# Boas vindas ao repositório backend do projeto de Deploy - Stranger Things!

Aqui você vai encontrar os locais para colocar suas repostas relativas aos requisitos de backend.

**Lembre-se**: coloque as respostas apenas dos requisitos que contém o seguinte direcionamento:

  - Adicione os comandos utilizados, de maneira sequencial, ao README do backend.

**Nota**: Este direcionamento está presente no [repositório](https://github.com/tryber/sd-01-block31-stranger-things) em que os requisitos do projeto são destrinchados.

## Requisitos

### 6 - Deploy Heroku

Para realizar o deploy do meu backend, fiz o seguinte procedimento:

`heroku create --remote hawkins stranger-things-backend`
`heroku create --remote upside-down st-backend-upside-down`

`heroku config:set UpsideDown=false --app stranger-things-backend`
`heroku config:set UpsideDown=true --app st-backend-upside-down`

`git add.`
`git commit -m "Acho que foi"`
`git push upside-down henrique-stranger-things-backend:master`
`git push hawkins henrique-stranger-things-backend:master`

### 7 - Monitoramento

Para conseguir realizar o monitoramento da minha API, fiz o seguinte procedimento:

`Adicione aqui os comandos utilizados, de maneira sequencial.`

`heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA" PM2_SECRET_KEY="CHAVE_PRIVADA" PM2_MACHINE_NAME=st-show --app stranger-things-backend`

`heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA" PM2_SECRET_KEY="CHAVE_PRIVADA" PM2_MACHINE_NAME=st-show --app st-backend-upside-down`
