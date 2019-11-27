# postgres

The docker-compose.yml file defines two services, Postgres and pgAdmin. The .env file defines all variables, this should be updated to reflect your requirements. 

To run the container, type the below command from the folder where your docker-compose.yml file is located:

`docker-compose up -d`

If you run the above code without the " -d " flag, the output will be displayed to the screen.

If you make changes to the docker-compose.yml file after you run the container for the firts time, you need to rebuild the container with the " --build " flag, eg.: `docker-compose up --build` 

To stop the container run:

`docker-compose down`

To access pgAdmin enter http://localhost in your browser. When promted, use the email address and password defined in you .env file



For additional variables and further information refer to [postgres](https://hub.docker.com/_/postgres) or [pgAdmin](https://www.pgadmin.org/docs/pgadmin4/4.13/container_deployment.html)


