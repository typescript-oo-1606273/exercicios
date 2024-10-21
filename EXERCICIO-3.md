# Exercício 3: Usando Classes e Interfaces

## Objetivo
Demonstrar o uso de `classes` para criar objetos com comportamentos e `interfaces` para definir a estrutura de um objeto em TypeScript, além de implementar diferentes comportamentos para métodos comuns.

## Instruções

1. Crie um projeto TypeScript e um arquivo `index.ts` na pasta `src`.

2. Crie uma interface chamada `Pessoa` com as seguintes propriedades e métodos:
   - `nome: string`
   - `idade: number`
   - `apresentar(): string` (método que deve retornar uma apresentação da pessoa).
   - `editarCurso(): boolean` (método que deve indicar se a pessoa pode editar um curso).

3. Crie uma classe chamada `Estudante` que implementa a interface `Pessoa` e adicione as seguintes propriedades:
   - `curso: string`

   A classe deve ter um construtor que aceita `nome`, `idade` e `curso`, além de implementar:
   - O método `apresentar()` retornando uma apresentação com nome, idade e curso.
   - O método `editarCurso()` que deve sempre retornar `false`.

4. Crie uma classe chamada `Professor` que também implementa a interface `Pessoa` e adicione as seguintes propriedades:
   - `materia: string`

   Assim como na classe `Estudante`, a classe deve ter um construtor que aceita `nome`, `idade` e `materia`, e deve implementar:
   - O método `apresentar()` retornando uma apresentação com nome, idade e matéria.
   - O método `editarCurso()` que deve sempre retornar `true`.

5. No arquivo `index.ts`, faça o seguinte:
   - Crie uma instância da classe `Estudante` e uma da classe `Professor`.
   - Exiba a apresentação de ambos utilizando o método `apresentar()`.
   - Verifique se cada um pode editar um curso utilizando o método `editarCurso()`.

OBS: crie as classes em arquivos separados, ex:
```bash
src/
├── index.ts
├── Pessoa.ts
├── Estudante.ts
└── Professor.ts
