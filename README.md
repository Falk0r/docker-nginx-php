# Server Nginx with PHP8.0

<img alt="Docker" src="https://walde.co/wp-content/uploads/2016/03/dockerphp.png">

This is a simple web server powered by Nginx and run php files with php8-0.

Yours codes is in the file "./code" and you can run the docker file with the command :
```sh
docker-compose up
```

The server is accessible to :
```sh
http://localhost:8080/
```

## PHP version
You can specify your version of PHP in the `.docker/Dockerfile` :
```Dockerfile
FROM php:8-fpm
```

And use the command :
```sh
docker-compose build
docker-compose up
```

## MySQL
- you also might want to adjust the default password (which is *"password"*) in `docker-compose.yml`
- port 3306
## phpmyadmin
- defaults see `docker-compose.yml`, also consider changing the password here too
- port [8082](http://localhost:8082)

