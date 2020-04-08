# Laravel Project Boilerplate

## Requirement
- PHP >= 7.x
- Docker
- Docker Compose 

## Setup
Clone this repository.
```shell
$ git clone git@github.com/kkznch/laravel-project-boilerplate.git
$ cd laravel-project-boilerplate
```

Copy `.env` file for docker compose.
```shell
$ cp .env.example .env
```

Create Laravel project.
You can change project directory name with `.env`.
```shell
$ composer create-project --prefer-dist laravel/laravel src
```

Edit `src/.env` for database access.
These are depends on `.env` for Docker Compose.
You can change these values with `.env`.
```diff:src/.env
- DB_HOST=127.0.0.1
+ DB_HOST=db
- DB_PASSWORD=
+ DB_PASSWORD=password
```

Build and run docker containers.
```shell
$ make up
```

Init application.
```shell
$ make app-init
```

# Documents 
## OpenAPI
Access to `http://localhost:8080`.

## DBDoc
Open the database document.
```sh
$ open ./document/dbdoc/README.md
```

Update database document.
```sh
$ make doc-db-update
```
