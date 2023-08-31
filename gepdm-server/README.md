## Como usar

```
yarn install
```

- Configure um database com Postgres e sete os dados num .env na raiz

```
// .env
PORT=3333
POSTGRES_HOST=localhost
DATABASE_URL=postgres://postgres:postgres@localhost:5432/your-database
ORM_CONFIG=development
POSTGRES_PORT=5432
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
POSTGRES_DB=your-database
SECRET_JWT_KEY=authentication_key
CLIENT_URL=http://localhost:3333
```

- Inicie o servidor

```
yarn dev
```

---


### Configuração do TypeORM

```
"typeorm:create": "yarn typeorm migration:create -n" // create a migration, add name of migration
"typeorm:revert": "yarn typeorm migration:revert" // drop table to generate new table
"typeorm:run": "yarn typeorm migration:run" // run migrations to create tables
```
