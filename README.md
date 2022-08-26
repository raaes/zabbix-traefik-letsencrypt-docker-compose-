# zabbix-traefik-letsencrypt-docker-compose-
# Install docker engine.
curl -fsSL get.docker.com -o get-docker.sh

sh get-docker.sh

Make sure the Docker Engine is installed correctly.

docker version

Add the user to the “docker” group using the command:

sudo usermod -aG docker $USER

# Installing zabbix:

Run zabbix-restore-database.sh to restore database if needed.

Deploy Zabbix server with a Docker Compose using the command(don't fogget to change all you need in "replace with yours":

docker compose -f zabbix-traefik-letsencrypt-docker-compose.yml -p zabbix up -d
