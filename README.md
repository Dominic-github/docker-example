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

#### mysql + phpadmin

```
cd mysql
cp .env.example .env
docker-compose -f mysql.docker-compose.yml up -d
```

#### redis

```
cd redis
cp .env.example .env
docker-compose -f mysql.docker-compose.yml up -d
```

#### mailhog

```
cd mailhog
cp .env.example .env
docker-compose -f mailhog.docker-compose.yml up -d
```

#### mongodb

```
cd mongodb
cp .env.example .env
docker-compose -f mongo.docker-compose.yml up -d
```

#### Laravel

- You need to put all the files into laravel or copy docker folder to your project.

Example:

```
laravel
│   │───app
│   │───bootstrap
│   │───config
│   │───database
│   │
│   │...
│   │
│   └─docker
│     │─── laravel.docker-compose.yml
│     │─── Dockerfile           # Change php version here
│     │─── .env.example         # Create your .env from example
│     └─── nginx
│                 └───default.conf  # Config nginx here
|
    ...
```

##### Run command

```
cd laravel
cp ./docker/.env.example ./docker/.env        # you can change port on .env

docker-compose -f laravel.docker-compose.yml up -d

```
