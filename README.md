# Cisco WEBEX API Commands


##### Exporta o token de autenticação do Webex para validar o usuario.
export TOKEN=Token 

##### Consome a API para enviar uma mensagem a um usuario especificado pelo parametro "toPersonEmail"
curl https://webexapis.com/v1/messages \
 -X POST -H "Authorization:Bearer $TOKEN" \
 -H "Content-Type: application/json" \
 --data '{"toPersonEmail":"EMAIL", "text":"Hi from Cisco"}'

##### Consome a API para criar uma sala no Webex. O nome da sala é especificado pelo parametro "title"
 curl https://webexapis.com/v1/rooms \
 -X POST -H "Authorization:Bearer $TOKEN" \
 -H "Content-Type: application/json" \
 --data '{"title":"NomeSala"}'
