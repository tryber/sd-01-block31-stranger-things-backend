# Boas vindas ao repositório backend do projeto de Deploy - Stranger Things!

Aqui você vai encontrar os locais para colocar suas repostas relativas aos requisitos de backend.

**Lembre-se**: coloque as respostas apenas dos requisitos que contém o seguinte direcionamento:

  - Adicione os comandos utilizados, de maneira sequencial, ao README do backend.

**Nota**: Este direcionamento está presente no [repositório](https://github.com/tryber/sd-01-block31-stranger-things) em que os requisitos do projeto são destrinchados.

## Requisitos

### 6 - Deploy Heroku

Para realizar o deploy do meu backend, fiz o seguinte procedimento:

`$heroku login`
`$heroku create --remote hawkings deploy-backend-hawkings-1234`
`$heroku config:set UPSIDEDOWN="false" --app deploy-backend-hawkings-1234`
`$heroku create --remote upside-down deploy-backend-upsidedown-1234`
`$heroku config:set UPSIDEDOWN="true" --app deploy-backend-upsidedown-1234`
`$git add / git commit`
`$git push hawkings MINHA-BRANCH:master`
`$git push upside-down MINHA-BRANCH:master`

### 7 - Monitoramento

Para conseguir realizar o monitoramento da minha API, fiz o seguinte procedimento:

##### - Hawkings:
`$heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA_AQUI" --app deploy-backend-hawkings-1234`
`$heroku config:set PM2_SECRET_KEY="CHAVE_PRIVADA_AQUI" --app deploy-backend-hawkings-1234`
`$heroku config:set PM2_MACHINE_NAME="NOME_SERVIDOR_HAWKINGS" --app deploy-backend-hawkings-1234`

##### - Upside-Down:
`$heroku config:set PM2_PUBLIC_KEY="CHAVE_PUBLICA_AQUI" --app deploy-backend-upsidedown-1234`
`$heroku config:set PM2_SECRET_KEY="CHAVE_PRIVADA_AQUI" --app deploy-backend-upsidedown-1234`
`$heroku config:set PM2_MACHINE_NAME="NOME_SERVIDOR_UPSIDEDOWN" --app deploy-backend-upsidedown-1234`
