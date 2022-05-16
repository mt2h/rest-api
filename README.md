# Rest API

# Example Case with need API Management

API in Real Life

![API in Real Life](./img/1.png)

![API in Real Life](./img/2.png)

API Consumers

![API Consumers](./img/3.png)

Add API Management

![Add API Management](./img/4.png)

API Consumers with API Management 

![API Consumers with API Management](./img/5.png)

Management

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
