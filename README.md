# Postgress and pgAdmin Container

The docker-compose.yml file defines two services, Postgres and pgAdmin. The .env file defines all variables, this should be updated to reflect your requirements. 
## Variables
- POSTGRES_USER
- POSTGRES_PASSWORD
- POSTGRES_DB
- PGADMIN_DEFAULT_EMAIL
- PGADMIN_DEFAULT_PASSWORD
- PGADMIN_DEFAULT_PORT
  - The default port for pgAdmin is port 80 but if you are running other servers on your local machine it may cause conflics so specifiy a different port if required, e.g.: 5050

## Running the containers
To run the container, type the below command from the folder where your docker-compose.yml file is located:

`docker-compose up -d`

If you run the above code without the " -d " flag, the output will be displayed to the screen.

If you make changes to the docker-compose.yml file after you run the container for the firts time, you need to rebuild the container with the " --build " flag, eg.: `docker-compose up --build` 

## Stopping the containers

To stop the container run:

`docker-compose down`

## Accessing pgAdmin

To access pgAdmin enter http://localhost in your browser, if you used a port other than port 80, you will need to access pgAdmin by going to http://localhost:port.
When promted, use the email address and password defined in you .env file

## Useful commands

To list running containers run ```docker ps ```

To run bash inside the container run ```docker exec -it CONTAINER_ID /bin/bash ```

To access a database from psql run ```psql --username usern_name --dbname postgres```

To list all databases type ``` \l+ ```

To create a database type ``` CREATE DATABASE database_name;``` 

To Connect to a database type ``` \c database_name  ```

For help type ``` \h ```

For additional variables and further information refer to [postgres](https://hub.docker.com/_/postgres) or [pgAdmin](https://www.pgadmin.org/docs/pgadmin4/4.13/container_deployment.html)


