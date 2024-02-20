<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

# NestJS API

# Ejecutar en Desarrollo
1. Clonar el repositorio
2. Ejecutar `npm install`
3. Tener NestJS CLI instalado `npm i -g @nestjs/cli`
4. Levantar la base de datos con `docker-compose up -d`
5. Clonar el archivo `.env.template` y renombrar la copia a `.env`
6. Llenar las variables de entorno en el archivo `.env`
7. Ejecutar `npm run start:dev`
8. Reconstruir la base de datos con `localhost:3000/api/v2/seed`

# Ejecutar en Producción
1. Clonar el repositorio
2. Crear el archivo `.env.prod` y llenar las variables de entorno
3. Crear nueva imagen `docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build`
4. Levantar la base de datos con `docker-compose -f docker-compose.prod.yaml --env-file .env.prod up -d`

## Stack Usado
- NestJS
- TypeORM
- MongoDB
- Docker
