# Postgres-Docker-Compose
Docker compose file that will initiate a local postgres-server with pgadmin4 to administrate it  
Access the web-version of PGAdmin4 via localhost:5050, no login needed  
Access to the database from PGAdmin4 is automatically set up, no need to do manualy

## Start/Stop:
Run the following command in a terminal in the repo to start
```bash
docker compose up -d
```
Run the following command in a terminal in the repo to stop
```bash
docker compose down
```
## Login information
All credetials can be changed in the docker-compose -file  

Using the web-version of pgadmin has the current credentials:
username: `user@mail.com`
password: `dbpass`  

Credentials to the postgres-server:
username: `postgres`
password: `dbpass`
