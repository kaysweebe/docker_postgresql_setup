# docker_postgresql_setup
Quickly put up a PostgreSQL database in a Docker container.

1. Get official Postgres image @ https://hub.docker.com/_/postgres
2. Go to terminal
3. Run `docker login` to login
4. Download image and run container `docker run --name my-postgres -p 5432:5432 -e POSTGRES_PASSWORD=mysecretpassword -d postgres`
5. Run `docker ps` and see if your container is running correctly

## Connecting to a database client
1. Setup new connection
2. Add host `localhost`
3. Add port `5432`
4. Add username `postgres`
5. Add password `mysecretpassword`
6. Test Connection

## Connecting to database through psql
1. Run `docker exec -it [container name or id here] /bin/bash`
2. Run `su - postgres`
3. Run `psql`
4. Do normal things like `\du` to see users from here!

