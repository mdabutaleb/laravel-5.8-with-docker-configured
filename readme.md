# Banglalink
Asset lite application

# Prerequisites
If you're very new with docker you can read [this](https://bitpress.io/simple-approach-using-docker-with-php/) awesome article. If you already have very basic idea about docker you may skip this step.

- [docker](https://www.docker.com/)
    - [Installation Guideline](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-18-04)
- [docker-compose](https://docs.docker.com/compose/) 
    ```
    sudo apt install docker-compose
    ```

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


# Development Resources
#### MySql 
```

mysql -u app -h 127.0.0.1 -P 16379 -p
```

