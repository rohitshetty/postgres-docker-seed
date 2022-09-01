### Postgres Docker Seed

Simple Docker compose script thingy that will load the output of pgdump (sql files) and bring up the instance.

### Running

0. Create a folder ./initdb.d
1. Drop the sql files inside ./initdb.d folder
2. Run `docker-compose up -d`
3. Check the status using `docker ps` (get the container id) +` docker logs CONTAINERID` and wait for the instance to complete the loading of data.
4. Connect with following connection string: `postgres://postgres:postgres_secret@localhost:9432/postgres` (Change in `docker-compose.yml` as needed)

This works based on this [Initialization details given here](https://hub.docker.com/_/postgres)
