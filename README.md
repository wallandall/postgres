# postgres

The docker-compose.yml file defines two services, Postgres and pgAdmin for. The .env file defines all variables, this should be updated to reflect your requirements. 

To run the container, type the below command from the folder where youur docker-compose.yml file is located:

`docker-compose up -d`

If you run the above code without the -d flag, the output will be displayed to the screen

After the container has been created you can run `docker-compose up --build` to rebuild the container with the updates

To stop the container run:

`docker-compose down`

To access pgAdmin enter http://localhost in your browser and the email address and password defined in you .env file

To access the postgress database type the below command  but ensure you replace the username and database name with the one defined in your .env file.

`psql -h localhost -p 54320 -U username -d database`

For more information refer to [pgAdmin](https://www.pgadmin.org/docs/pgadmin4/4.13/container_deployment.html)


