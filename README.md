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
docker-compose ps
```

Commands Docker Compose

```bash
#Create all containers, without start them.
docker-compose up --no-start

#Start all containers.
docker-compose start

#Stop all running containers.
docker-compose stop
```

view kong
http://localhost:8001

view konga
http://localhost:1337

view service example
http://locky:9001/

Docker Network Kong

![Docker Network Kong](./img/7.png)

Use Postman to use Kong

Set Environment Kong

![Se Environment Kong](./img/8.png)

Get in API Kong

![Get in API Kong](./img/9.png)

## Ports Kong

![Ports Kong](./img/11.png)


## Kong Services

Add Service

![Add Service](./img/10.png)

## Kong Routes

Add Route

![Add Route](./img/16.png)

http://localhost:8000/qr
http://goqr.me/api/doc/
http://momo:8000/qr/v1/create-qr-code/?data=Hello

Service QR in Kong

![Service QR in Kong](./img/12.png)

### Update Endpoint Service


![Update Endpoint Service](./img/13.png)


![Schema Update Endpoint Service](./img/14.png)

## Kong Consumers

Add Consumers

![Add Consumers](./img/17.png)

![Schema Consumers](./img/15.png)
