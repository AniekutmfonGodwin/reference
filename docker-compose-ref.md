## how to setup replica in docker compose

    services:
      app:
        image: nginx
        deploy:
          mode: replicated
          replicas: 2 
      backend:
        image: mysql:5.7
        volumes:
          - data:/var/lib/mysql
        restart: always
        environment:
          MYSQL_ROOT_PASSWORD: set
          MYSQL_DATABASE: set
          MYSQL_USER: set
          MYSQL_PASSWORD: set

    volumes: 
      data: {}
