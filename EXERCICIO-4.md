# Exercício 4: Usando Classes e Interfaces

## Objetivo
Demonstrar o uso de `classes` para criar objetos com comportamentos e `interfaces` para definir a estrutura de um objeto em TypeScript.

## Instruções

1. Crie um projeto TypeScript e um arquivo `index.ts`.

2. Crie uma interface chamada `Pessoa` com as seguintes propriedades:
   - `nome: string`
   - `idade: number`
   - `apresentar(): string` (método que deve retornar uma apresentação da pessoa).

3. Crie uma classe chamada `Estudante` que implementa a interface `Pessoa` e adicione as seguintes propriedades:
   - `curso: string`

   A classe deve ter um construtor que aceita `nome`, `idade` e `curso`, além de implementar o método `apresentar()`.

4. Crie uma classe chamada `Professor` que também implementa a interface `Pessoa` e adicione as seguintes propriedades:
   - `materia: string`

   Assim como na classe `Estudante`, a classe deve ter um construtor que aceita `nome`, `idade` e `materia`, e implementar o método `apresentar()`.

5. No arquivo `index.ts`, faça o seguinte:
   - Crie uma instância da classe `Estudante` e uma da classe `Professor`.
   - Exiba a apresentação de ambos utilizando o método `apresentar()`.

EXTRA: Separe `Pessoa`, `Estudante` e `Professor` em diferentes arquivos utilizando `export` e `import`.
