<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest


# nest CLI

```bash
nest g resource users
```


# app.module

```ts
imports: [
    TypeOrmModule.forRoot({
      type: 'sqlite', // nome do db
      database: 'db.sqlite', // credenciais de acesso
      entities: ['dist/**/*.entity.js'], //caminho onde sera criada as entidades
      synchronize: true, // se (True), cria automaticamente as schemas
    }),
    UsersModule,
  ],
  ```