Database with persistance `Data` container
===
## Includes MySql, Postgres, Redis, Memcached

This is inspired from: [https://github.com/LaraDock/laradock](https://github.com/LaraDock/laradock)

### Start all containers

	$ docker-compose up -d

### Start only needed containers

	$ docker-compose up -d mysql

### Stop running containers

	$ docker-compose stop

### Remove containers

    $ docker-compose down

**NOTE:** Data is not automatically removed from the data container

This will list the volumes that are not used:

	$ docker volume ls -f dangling=true

If you want to cleanup data volumes run:

	$ docker volume rm $(docker volume ls -qf dangling=true)

**NOTE:** If you remove the `Data` container and start it again it will re-use the old volume so **no data is lost**
