# Exercício 3: Criando uma API com Node.js e TypeScript sem Frameworks

## Objetivo
Criar uma API básica utilizando **Node.js** e **TypeScript**. A API irá responder com um texto em uma requisição HTTP.

## Instruções

### 1. Criar o diretório do projeto e inicializar o npm
```bash
mkdir minha-api-typescript
cd minha-api-typescript
npm init -y
```

### 2. Instale as ferramentas necessárias no projeto
```bash
npm install typescript ts-node @types/node --save-dev
```

### 3. Configure o Typescript no projeto
```bash
npx tsc --init
```

Arquivo tsconfig.json:

```json
{
  "compilerOptions": {
    "outDir": "./dist",
    "rootDir": "./src",
    "strict": true,
    "esModuleInterop": true
  }
}
```

### 4. Criar a API

No diretório src, crie um arquivo server.ts

```bash
mkdir src
touch src/server.ts
```

No arquivo server.ts, escreva o código da API:

```typescript
import { createServer, IncomingMessage, ServerResponse } from 'http';

// Função para lidar com as requisições HTTP
const route = (req: IncomingMessage, res: ServerResponse) => {
  res.writeHead(200, { 'Content-Type': 'text/plain' });
  res.end('Olá, mundo! Esta é uma API Node.js com TypeScript puro.');
};

// Criar o servidor HTTP
const server = createServer(route);

// Iniciar o servidor na porta 3000
server.listen(3000);
```

### 4. Crie os comandos necessários para rodar o servidor

Abra o arquivo package.json e adicione o seguinte script para rodar o servidor:

```json
"scripts": {
  "dev": "ts-node src/server.ts",
}
```

### 5. Rodar o servidor

Execute o comando `npm run dev` e acesse a api em `http://localhost:3000`

