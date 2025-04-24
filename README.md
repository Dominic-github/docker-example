# 🐳 Docker Example

## Requirement

- docker
- docker-compose

## Install

```
git clone https://github.com/dominic-github/docker-example
cd docker-example
```

### How to run?

mysql + phpadmin

```
cd mysql
cp .env.example .env
docker-compose -f mysql.docker-compose.yml up -d
```

redis

```
cd redis
cp .env.example .env
docker-compose -f mysql.docker-compose.yml up -d
```

mailhog

```
cd mailhog
cp .env.example .env
docker-compose -f mailhog.docker-compose.yml up -d
```

mongodb

```
cd mongodb
cp .env.example .env
docker-compose -f mongo.docker-compose.yml up -d
```
