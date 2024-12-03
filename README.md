# Laravel 7 with Docker

up services

```sh
docker-compose up -d
```

down services

```sh
docker-compose down
```

create laravel project

```sh
# connect to container
docker exec -it $(name of container) bash

# run bash in the container
composer create-project --prefer-dist laravel/laravel:^7.0

# add permissions (optional if the above returns an error)
chmod -R 777 storage/
```

modify .env file for your db config

```sh
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=your_db
DB_USERNAME=your_user
DB_PASSWORD=your_password
```
