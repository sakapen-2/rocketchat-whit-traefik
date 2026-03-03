mkdir letsencrypt
touch letsencrypt/acme.json
chmod 600 letsencrypt/acme.json
docker compose -f docker-compose.yml up -d 
