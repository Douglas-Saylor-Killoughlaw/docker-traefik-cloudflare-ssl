# docker-traefik-cloudflare-ssl
Roll up a web server with docker, traefik, cloudflare

# Create traefik basic auth user and password
`echo $(htpasswd -nb user password) | sed -e s/\\$/\\$\\$/g`

# ACME SETUP
(INITIAL - CLEANING)
`cd configs && >acme.json`

(Correct Permissions)
`chmod ./configs/acme.json`

# RUN
`docker-compose up -d`

# logs
`docker-compose logs -f`

# stop
`docker-compose stop`

