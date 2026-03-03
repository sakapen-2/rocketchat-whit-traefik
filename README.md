mkdir letsencrypt

touch letsencrypt/acme.json

chmod 600 letsencrypt/acme.json

docker network create web

docker compose -f docker-compose.yml up -d 

docker compose -f compose-rocket.yml -f database.yml  up -d 
