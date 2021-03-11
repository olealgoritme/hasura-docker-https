# hasura-docker-https
- dockerized postgres + hasura + graphql setup
- caddy for automated letscrypt certificates and reverse proxy for https for a set domain

- setup steps for ubuntu server
```
git clone https://github.com/olealgoritme/hasura-docker-https
cd hasura-docker-https
sudo ./setup.sh
vim docker-compose.yaml [replace ADMIN-SECRET-KEY]
vim Caddyfile [replace domain]
docker-compose up -d
docker-compose restart caddy
```

