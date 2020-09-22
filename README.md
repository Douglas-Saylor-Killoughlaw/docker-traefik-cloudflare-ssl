# docker-traefik-cloudflare
Roll up a web server with docker, traefik, cloudflare

# Create traefik basic auth user and password
echo $(htpasswd -nb user password) | sed -e s/\\$/\\$\\$/g

# RUN
docker-compose up -d

# logs
docker-compose logs -f

# stop
docker-compose stop

