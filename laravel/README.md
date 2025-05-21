# Laravel

- You need to put all the files into laravel.

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

Run command

```
cd laravel
cp ./docker/.env.example ./docker/.env        # you can change port on .env

docker-compose -f laravel.docker-compose.yml up -d

```
