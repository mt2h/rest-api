# Rest API

## Run dependences

```bash
docker run -it --rm --name rabbitmq -p 15672:15672 -p 5672:5672 rabbitmq:3-management
#http://localhost:15672
#guest guest
```

## Install Docker Compose

```bash
sudo curl -L "https://github.com/docker/compose/releases/download/v2.5.0/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
sudo chmod +x /usr/local/bin/docker-compose
docker-compose --version
```

## Run Kong

```bash
docker-compose up -d
```