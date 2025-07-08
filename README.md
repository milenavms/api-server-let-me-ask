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

### Executando o Servidor

```sh
npm run dev
```

Ou, para buildar e rodar:

```sh
npm run build
npm start
```

## Estrutura do Projeto


## Licença

[MIT](LICENSE)
