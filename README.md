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
http://localhost:9001/

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
http://localhost:8000/qr/v1/create-qr-code/?data=Hello

Service QR in Kong

![Service QR in Kong](./img/12.png)

### Update Endpoint Service


![Update Endpoint Service](./img/13.png)


![Schema Update Endpoint Service](./img/14.png)

## Kong Consumers

Add Consumers

![Add Consumers](./img/17.png)

![Schema Consumers](./img/15.png)

## Konga

http://localhost:1337/register

Conexion with Kong

![Conexion with Kong](./img/18.png)

Add Service

![Add Service](./img/19.png)

Add Route on Service

![Add Route on Service](./img/20.png)

View Route on Service on Web Browser

![View Route on Service on Web Browser](./img/21.png)

Add Consumer

![Add Consumer](./img/22.png)

Documentation: https://pantsel.github.io/konga/

Add User

![Add User](./img/23.png)

Take Snapshot Backup

![Take Snapshot Backup](./img/24.png)

Restore from file Snapshot

![Restore from file Snapshot](./img/25.png)

Sheduler Snapshot Backup

![Sheduler Snapshot Backup](./img/26.png)

## HealthCheck and LoadBalancer

![Upstream and Target](./img/27.png)

![HealthCheck](./img/28.png)

![LoadBalancer Weighted Round Robin](./img/29.png)

![LoadBalancer Hash based](./img/30.png)

![LoadBalancer + HealthCheck](./img/31.png)

### Upstream

In Konga

![Create Upstream](./img/32.png)

![Add Target to Upstream](./img/33.png)

![Edit HealthCheck of Upstream](./img/34.png)

In Postman

![Create Upstream in Postman](./img/35.png)

![Add Target to Upstream in Postman](./img/36.png)

Current Schema

![Current Schema](./img/37.png)

Change Host Service by Upstream

![Change Host Service by Upstream](./img/38.png)

### Enable Alerts of Slack

![Enable Alerts of Slack 1](./img/39.png)

![Enable Alerts of Slack 2](./img/40.png)

![Enable Alerts of Slack 3](./img/41.png)

![Enable Alerts of Slack 4](./img/42.png)

![Enable Alerts of Slack 5](./img/43.png)

![Enable Alerts of Slack 6](./img/44.png)

![Enable Alerts of Slack 7](./img/45.png)

![Enable Alerts from Konga](./img/46.png)

## Services & API

### Service Alfa

* Base URL: http://localhost/alpha
* List of available endpoints: Alpha http://localhost/alpha/swagger-ui.html

### Service Beta

* Base URL: http://localhost/beta
* List of available endpoints: Alpha http://localhost/beta/swagger-ui.html

### Service Gamma

* Base URL: http://localhost/gamma
* List of available endpoints: Alpha http://localhost/gamma/swagger-ui.html

### Service Omega

* Base URL: http://localhost/omega
* List of available endpoints: Alpha http://localhost/omega/swagger-ui.html

## Plugin Basic Authentication on Konga

![Plugin Basic Authentication on Konga](./img/47.png)

![Basic Authentication For User](./img/48.png)

![Basic Authentication whith Postman](./img/49.png)

## Plugin API Key on Konga

Add API Key on an Service

![Add API Key on an Service](./img/50.png)

![Add API Key on an Service](./img/51.png)

![Apy Key to User](./img/52.png)

![Using Apy Key to Request on Postman](./img/53.png)

## Plugin HMAC on Konga

![Add HMAC on an Service](./img/54.png)

![Add HMAC to User](./img/55.png)

Generator: https://dinochiesa.github.io/hmachash/index.html

![HMAC Codification](./img/56.png)

![Using HMAC to Request on Postman](./img/57.png)