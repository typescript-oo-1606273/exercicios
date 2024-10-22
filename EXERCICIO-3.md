# Exercício 3: Usando Classes

## Objetivo
Demonstrar o uso de `classes` para criar objetos com comportamentos em TypeScript, além de implementar diferentes comportamentos para métodos comuns.

## Instruções

1. Crie um projeto TypeScript e um arquivo `index.ts` na pasta `src`.

2. Crie uma classe chamada `Estudante` com as seguintes propriedades:
   - `nome: string`
   - `idade: number`
   - `curso: string`

   A classe deve ter um construtor que aceita `nome`, `idade` e `curso`, além de implementar:
   - Um método `apresentar()` que retorna uma apresentação com nome, idade e curso.
   - Um método `editarCurso()` que sempre retorna `false`.

3. Crie uma classe chamada `Professor` com as seguintes propriedades:
   - `nome: string`
   - `idade: number`
   - `materia: string`

   A classe deve ter um construtor que aceita `nome`, `idade` e `materia`, além de implementar:
   - Um método `apresentar()` que retorna uma apresentação com nome, idade e matéria.
   - Um método `editarCurso()` que sempre retorna `true`.

4. No arquivo `index.ts`, faça o seguinte:
   - Crie uma instância da classe `Estudante` e uma da classe `Professor`. Ex:
     ```typescript
     const joao = new Estudante("João", 30, "Typescript");
     const jeff = new Professor("Jefferson", 29, "Typescript");
     ```
   - Exiba a apresentação de ambos utilizando o método `apresentar()`.
   - Chame o método `editarCurso()` em cada um dos objetos e mostre no console.
