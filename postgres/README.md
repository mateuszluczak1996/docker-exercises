## Exercise - Setup postgres database along with admin panel

1. Postgress image
 * all useful information are on docker hub: [postgres-docker-hub](https://hub.docker.com/_/postgres)
 * only required enviroment field is POSTGRES_PASSWORD
 * data is stored in `/var/lib/postgresql/data` folder by default. That's why I create volume with that path

2. Adminer image
* all useful information are on docker hub: [adminer-docker-hub](https://hub.docker.com/_/adminer)
* port is mapped from container 8080 to port 8080 on the Docker host in order to have an access on the local machine.