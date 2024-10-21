# Exercício: Iniciando um projeto Typescript e lidando com tipos

## Objetivo
- Configurar o ambiente TypeScript e garantir que o código seja corretamente compilado e executado.
- Demonstrar conhecimento de tipos básicos em TypeScript (number, string, boolean) e o uso de funções com parâmetros tipados.

## Instruções:

- Crie um novo diretório e inicialize o projeto:
  ```bash
  mkdir exercicio-1
  cd exercicio-1
  npm init -y

- Instale o typescript no projeto:
  ```bash
  npm install typescript --save-dev

- Configure o typescript:
  ```bash
  npx tsc --init

- Faça as modificações que achar necessário no arquivo tsconfig.json.  
- No diretório src, crie um arquivo chamado index.ts.
- Crie uma função com parâmetros tipados (number, string, boolean, etc.). Ex:
  ```typescript
  function apresentar(nome: string): string {
    return `Prazer, sou ${nome}!`;
  }
  ```
- Defina variáveis com os tipos string, number e boolean e um objeto qualquer.
- Exiba o valor dessas variáveis no console.
- Chame a função criada e mostre o resultado no console. Ex:
  ```typescript
  console.log(apresentar("Jeff");
  ```

- Compile o código criado
  ```bash
  tsc
  ```
- Execute o código Javascript gerado
  ```bash
  node src/index.js
  ```


