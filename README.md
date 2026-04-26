# Postgres-Docker-Compose
Docker compose file that will initiate a local postgres-server with pgAdmin4 to administrate it  
Access the web-version of pgAdmin4 via localhost:5050, no login needed  
Access to the database from pgAdmin4 is automatically set up, no need to do manually  
The postgresql container runs the latest postgresql version. (Should there be issues, try changing from `latest` to `17`)  
The pgAdmin4 container runs the lastest pgAdmin4 version.

## Start/Stop:
Run the following command in a terminal in the directory to start
```bash
docker compose up -d #To start both services
docker compose up -d postgres #To only start the postgres-server
docker compose up -d pgadmin #To only start the pgadmin web-application
```
Run the following command in a terminal in the directory to stop
```bash
docker compose down
```
## Login information
All credetials can be changed in the docker-compose -file   (all can of course be changed in the `docker-compose.yml`-file)

Using the web-version of pgadmin has the current credentials:
- username: `user@mail.com`
- password: `dbpass`  

Credentials to the postgres-server:
- username: `postgres`
- password: `dbpass
