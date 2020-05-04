# Docker LAMP for noobs

The repo consist of docker-compose setup to run LAMP stack based on [mattrayner/docker-lamp](https://hub.docker.com/r/mattrayner/lamp).

## Run & Install
* Change the `.env` file to match your setting
* Start Container : `docker-compose up -d`
* Stop Container : `docker-compose down`

## Add docker-compose as a system Service 
* `cp docker-lamp.service /etc/systemd/system/docker-lamp.service`
* `systemctl daemon-reload`
* `systemctl start docker-lamp`
* `systemctl enable docker-lamp` 

## MySQL

Default username is `admin` and you can set the password via `.env` file.