### Postgres Docker Seed

Simple Docker/Docker compose script thingy that will load the output of pgdump and bring up the instance.

### Running

1. Drop the out of the file in ./data folder
2. Run `docker-compose up -d`
3. Check the status using `docker ps + docker logs` and wait for the instance to complete the loading of data.
