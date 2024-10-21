# EXTRA: Criando uma API com Node.js e TypeScript sem Frameworks

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
npm install typescript ts-node express @types/express --save-dev
```

### 3. Configure o Typescript no projeto
```bash
npx tsc --init
```

Ajuste o arquivo tsconfig.json:

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

No arquivo server.ts, escreva o código da API:

```typescript
import * as express from 'express';

const app = express();

app.get('/', (request, response) => {
  response.json({
    nome: "Jefferson",
    idade: 29
  });
})

app.listen(3000, () => {
  console.log("API Rodando na port 3000");
});
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

