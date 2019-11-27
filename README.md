# postgres

This file defines two services, Postgres and pgAdmin for. The variables are defined in the .env file and should be updated to reflect your requirements. 

To run the container, type the below command from the folder where youur docker-compose.yml file is located
`docker-compose up -d`

To stop the container run:
`docker-compose down`

To access pgAdmin enter http://localhost in your browser and the email address and password defined in you .env file

To access the postgress database type the below command from the folder wher your docker-compose.yml file is located. Replace the username and database name with the one defined in your .env file.
`psql -h localhost -p 54320 -U username -d database`
