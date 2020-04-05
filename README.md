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

Copy `.env` file.
```shell
$ cp .env.example .env
```

Create Laravel project.
```shell
$ composer create-project --prefer-dist laravel/laravel src
```

Build and run docker containers.
```shell
$ make up
```

Init application.
```shell
$ make app-init
```

# Other Documents 

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
