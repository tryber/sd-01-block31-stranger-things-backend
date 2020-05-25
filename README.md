# Boas vindas ao repositório backend do projeto de Deploy - Stranger Things!

Aqui você vai encontrar os locais para colocar suas repostas relativas aos requisitos de backend.

**Lembre-se**: coloque as respostas apenas dos requisitos que contém o seguinte direcionamento:

  - Adicione os comandos utilizados, de maneira sequencial, ao README do backend.

**Nota**: Este direcionamento está presente no [repositório](https://github.com/tryber/sd-01-block31-stranger-things) em que os requisitos do projeto são destrinchados.

## Requisitos

### 6 - Deploy Heroku

Para realizar o deploy do meu backend, fiz o seguinte procedimento:

`Adicione aqui os comandos utilizados, de maneira sequencial.`

heroku create --remote hawkins
heroku config:set upsideDown="false" --app morning-reaches-10338
heroku create --remote upside-down
heroku config:set upsideDown="true" --app evening-waters-77718
git add .
git commit -m 'Meu primeiro deploy no Heroku!'
git push hawkins master
git push upside-down master

### 7 - Monitoramento

Para conseguir realizar o monitoramento da minha API, fiz o seguinte procedimento:

pm2 link "CHAVE_PRIVADA_AQUI" 0f6fab5hd74n3qr
pm2 plus
`Adicione aqui os comandos utilizados, de maneira sequencial.`
