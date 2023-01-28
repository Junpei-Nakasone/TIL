
docker-compose.yml
```yml
version: '3'
services:
  db:
    image: mysql:8.0.23

    environment:
      - MYSQL_ROOT_HOST=${DB_ROOT_HOST}
      - MYSQL_DATABASE=${DB_NAME}
      - MYSQL_USER=${DB_USER}
      - MYSQL_PASSWORD=${DB_PASS}
      - MYSQL_ROOT_PASSWORD=${DB_PASS}
      - TZ=${TZ}
    # environment variables also can be defined by 'env_file' property which specify the path where .env exists.


    # host port:container port
    ports:
      - '3306:3306'

    volumes:
      - ./db/conf:/etc/mysql/conf.d/:ro
      # put the initial data on /docker-entrypoint-initdb.d
      # https://hub.docker.com/_/mysql
      - ./db/init:/docker-entrypoint-initdb.d
      - ./db/logs:/var/log/mysql

    networks:
      - backend
networks:
  backend:

```

.env
```
DB_ROOT_HOST=%
DB_NAME=example_db
DB_USER=example_username
DB_PASS=example_password
TZ=Asia/Tokyo
```
