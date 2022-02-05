# Launching project

<hr>

## Project description

- Backend - Symfony 5, PHP 8, Doctrine ORM
- Frontend - Angular
- Database - MySQL

## Exposed ports

- backend - `8000`
- frontend - `4200`
- mysql - `3306`
- phpmyadmin - `8080`

## Requirements

- Docker
- docker-compose
- PHP `8.0`
- Symfony CLI (optional - replace commands `symfony *` with `php bin/console *`)

## Project preparation

1. Build docker containers
```bash
docker-compose up -d
```
2. When containers are ready go to `backend` directory
```bash
cd backend
```
3. Make database migrations
```bash
symfony console doctrine:migrations:migrate
```
4. Launch Symfony local web server
```bash
symfony server:start
```
5. Enjoy frontend on local webpage `http://localhost:4200`
