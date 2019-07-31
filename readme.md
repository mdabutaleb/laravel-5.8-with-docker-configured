# Laravel 5.8 with Docker configured
This is completely fresh laravel 5.8 application with docker configured. If you're looking for make your laravel project dockerize then this project will save your time. Because it's ready with docker configured !
# Prerequisites
If you're very new with docker you can read [this](https://bitpress.io/simple-approach-using-docker-with-php/) awesome article. If you already have very basic idea about docker you may skip this step.

- [docker](https://www.docker.com/)
    - [Installation Guideline](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04)
- [docker-compose](https://docs.docker.com/compose/) 
    ```
    sudo apt install docker-compose
    ```
### Environment you'll get
1. PHP 7.2
2. MySQL 5.7
3. Laravel 5.8

# Installation
#### Run commands after initial pull

```
composer install
chmod -R o+rw bootstrap/ storage/ 
```  

*To build and run docker image*
```
docker-compose up --build
```

*To run docker image*
```
docker-compose up
```

*To run docker image in background*
```
docker-compose up -d
```

*Access application*

[http://localhost:8081](http://localhost:8081)



# Development Resources
#### MySql 
```

mysql -u app -h 127.0.0.1 -P 16379 -p
```

