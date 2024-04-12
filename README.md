<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation
1. Clonar el repositorio
2. ejecutar
```bash
$ yarn install
```
3. Tener Nest CLI instalado
```bash
$ npm i -g @nestjs/cli
```
4. Crear un proyecto
```bash
$ nest new <project name>
$ cd <project name>
```
5. Levantar la BD
```bash
# Descargar imagen de Mongo 5.0.0 y postgres 14
$ docker pull mongo:5.0.0
# Crear nuevo archivo docker-compose.yaml
$ docker-compose up -d
```

6. Agregar Nest - modern, fast, powerful node.js web framework (@mongoose)
```bash
# A progressive Node.js framework for building efficient and scalable server-side applications
$ yarn add @nestjs/mongoose mongoose
```
7. Agregar Validators

```bash
# Agrega librerías externas útiles. Algunos decoradores de Class Validator: @IsString(), @MinLength(1)
$ yarn add class-validator class-transformer
# Agrega Configuración global de pipes en main.ts
```




## Stack usado
* MongoDB
* Nest


## Running the app

```bash
# development
$ yarn run start

# watch mode
$ yarn run start:dev

# production mode
$ yarn run start:prod
```
## Running Html static
```bash
# development
$ yarn add @nestjs/serve-static
# agregar en app.module.ts
@Module({
  imports: [ServeStaticModule.forRoot({
    rootPath: join(__dirname,'..','public'),
    })],
})
```
## Crear REST API

```bash
# development
$ nest g res <nombre> --no-spec
? Would you like to generate CRUD entry points? (Y/n) Y
```

## Crear Modulo

```bash
# development
$ nest g mo <nombre> #ej. nest g mo common

```
## Crear Pipe

```bash
# development
$ nest g pi <Path>/<nombre> --no-spec #ej. nest g pi common/pipes/parseMongoId --no-spec

```

## Test

```bash
# unit tests
$ yarn run test

# e2e tests
$ yarn run test:e2e

# test coverage
$ yarn run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).
