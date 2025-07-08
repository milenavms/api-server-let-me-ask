# Let Me Ask - API Server

Este é o backend da aplicação Let Me Ask, desenvolvido com Node.js e TypeScript.

## Funcionalidades

- Projeto inicializado com Node.js e TypeScript

## Primeiros Passos

### Pré-requisitos

- Node.js 22.x (recomendado)
- npm ou yarn
- Docker e Docker Compose

### Instalação

Clone o repositório e instale as dependências:

```sh
git clone https://github.com/milenavms/api-server-let-me-ask.git
cd api-server-let-me-ask
npm install
```

### Subindo o Banco de Dados com Docker

Execute o comando abaixo para iniciar o banco de dados PostgreSQL com a extensão pgvector:

```sh
docker compose up -d
```

### Gerando as Migrations com Drizzle Kit

Após configurar o banco e o schema, gere as migrations com:

```sh
npx drizzle-kit generate
```
Será criado na pasta src/db/migrations

### Rodando as Migrations

Para aplicar as migrations ao banco de dados, execute:

```sh
npx drizzle-kit migrate
```

### Rodando o Seed de Dados

Para pré-popular o banco de dados com dados fictícios, execute:

```sh
npm run db:seed
```

### Acessando o Drizzle Studio

Para visualizar e gerenciar o banco de dados de forma gráfica, utilize o Drizzle Studio:

```sh
npx drizzle-kit studio
```

Acesse o https://local.drizzle.studio

### Executando o Servidor

```sh
npm run dev
```

Ou, para buildar e rodar:

```sh
npm run build
npm start
```

# Health Check

A rota abaixo pode ser utilizada para verificar se o serviço está no ar:

```ts
app.get('/health', () => {
  return 'ok';
});
```

Acesse em: http://localhost:3333/health



## Estrutura do Projeto


## Licença

[MIT](LICENSE)
