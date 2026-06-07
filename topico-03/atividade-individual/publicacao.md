# Publicação do site

## Nível escolhido
Nível 2 - Intermédio

## Rota escolhida
Nginx

## Ficheiros criados
- index.html
- sobre.html
- style.css

## Local de publicação
/var/www/html/topico-03/

## Comandos principais utilizados
- sudo apt install nginx -y
- sudo mkdir /var/www/html/topico-03
- sudo cp site/* /var/www/html/topico-03/
- sudo ufw allow 80/tcp

## Resultado obtido
Site publicado e acessível no browser e via url.

## Limitações encontradas
A porta 80 não estava aberta no firewall — resolvido com ufw allow 80/tcp.
