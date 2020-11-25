# Introduction
This is basic a scaffolding to run php application with docker. This includes ```nginx```, ```php7.4-fpm```, ```mariadb-10.3.23```, ```redis-6.0.5``` and ```phpmyadmin``` 

## Installation
```
git clone https://github.com/rushdasoftbd/php-with-docker.git my-project
cd my-project
mkdir src
```
Replace ```my project``` with your ```project name```. ```src``` folder will contain your php project. and ```web root``` will be ```src/public```

open ```docker-compose.yml``` file and replace ```project-name``` with your ```project name```

Create ```cert-key.pem``` and ```cert.pem``` file on ```.docker/nginx/ssl``` directory. Help <https://github.com/majorsabbir/docker-laravel8#ssl-certificate>

Run
```
docker-compose build
docker-compose up -d
```

To view ```application``` on browser <https://localhost>, and for ```phpmyadmin``` <localhost:7000>