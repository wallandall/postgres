# postgres

The docker-compose.yml file defines two services, Postgres and pgAdmin for. The .env file defines all variables, this should be updated to reflect your requirements. 

To run the container, type the below command from the folder where youur docker-compose.yml file is located:

`docker-compose up -d`

If you run the above code without the -d flag, the output will be displayed to the screen

After the container has been created you can run `docker-compose up --build` to rebuild the container with the updates

To stop the container run:

`docker-compose down`

To access pgAdmin enter http://localhost in your browser and the email address and password defined in you .env file



For more information refer to [postgres](https://hub.docker.com/_/postgres) or [pgAdmin](https://www.pgadmin.org/docs/pgadmin4/4.13/container_deployment.html)


