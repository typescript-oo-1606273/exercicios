# Exercício: Classificação de Idades

## Objetivo

Criar um programa simples que classifique uma pessoa de acordo com sua idade, utilizando conceitos básicos de TypeScript, como tipos primitivos, type aliases, enums e funções.

## Instruções

1. **Criar um Enum para as Faixas Etárias**

   - Defina um `enum` chamado `CategoriaIdade` com os seguintes valores:
     - `CRIANCA` (0 a 12 anos)
     - `ADOLESCENTE` (13 a 17 anos)
     - `ADULTO` (18 a 64 anos)
     - `IDOSO` (65 anos ou mais)

2. **Criar um Tipo para Representar uma Pessoa**

   - Defina um `type` chamado `Pessoa`, contendo:
     - `nome`: string
     - `idade`: number

3. **Criar uma Função para Classificar a Idade**

   - Crie uma função que receba um objeto do tipo `Pessoa` e retorne a categoria correspondente da idade.

4. **Testar o Programa**
   - Crie algumas pessoas de diferentes idades e exiba a classificação no console.
