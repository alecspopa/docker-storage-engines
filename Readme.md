Database with persistent `data` volumes
===
## Includes MariaDB, MySql 5.7, Postgres, Redis, Memcached

This is inspired from: [https://github.com/LaraDock/laradock](https://github.com/LaraDock/laradock)

### Start all containers

	$ docker-compose up -d

### Start only needed containers

	$ docker-compose up -d mysql

### Stop running containers

	$ docker-compose stop

### Remove containers

	$ docker-compose down
