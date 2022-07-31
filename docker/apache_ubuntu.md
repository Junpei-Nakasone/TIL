
docker pull ubuntu:latest

docker run -d --name web_server_test -p 127.0.0.1:80:80 ubuntu:latest


docker ps

docker attach [containerID]


Inside Container

apt-get update

apt-get install apache2

service apache2 status
not running yet

service apache2 start

service apache2 status
running

(you can see apache welcome page by accessing 127.0.0.1)

apt-get install curl

curl localhost
you will see apache html data.
