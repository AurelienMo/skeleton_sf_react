# Docker stack SF + React

## Run project
- Define variables in docker/.env file
- Launch project   
`docker-compose up --env-file docker/.env --build (you can add -d option to launch in background)`

## Launch API

- `composer install` from "www"" container
- Copy `.env` to `.env.local` and define all necessary variables, especially DATABASE_URL to match configuration define in `docker/.env` file  
- API can be accessible on url `https://localhost` (auto signed ssl certificate)

## Launch front

- `npm install` from "frontreact" container
- `HTTPS=true npm start` from "frontreact" container
- front can be accessible on url `https://localhost:3001`
