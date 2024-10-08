# Exercício 4: Criando um Projeto TypeScript com Vite e React

## Objetivo
Aprender a criar um projeto React com TypeScript utilizando o **Vite**, uma ferramenta de build rápida para projetos modernos. Este exercício ajuda a configurar um ambiente React com TypeScript desde o início e a publicar a aplicação.

## Instruções

1. **Criar o projeto com Vite:**
   - No terminal, navegue até o diretório onde deseja criar o projeto.
   - Execute o seguinte comando para criar um novo projeto Vite com suporte a React e TypeScript:
     ```bash
     npm create vite@latest meu-projeto -- --template react-ts
     ```
   - Entre no diretório do projeto:
     ```bash
     cd meu-projeto
     ```

2. **Instalar as dependências:**
   - Instale as dependências do projeto:
     ```bash
     npm install
     ```

3. **Executar o projeto:**
   - Inicie o servidor de desenvolvimento com o Vite:
     ```bash
     npm run dev
     ```
   - O projeto estará rodando localmente. Acesse o link fornecido no terminal (normalmente `http://localhost:5173`) para visualizar a aplicação.

4. **Modificar o código:**
   - No diretório `src`, abra o arquivo `App.tsx`.
   - Edite o arquivo para incluir um layout HTML simples.

5. **Criar o estilo CSS:**
   - No diretório `src`, abra o arquivo `App.css`.
   - Edite o arquivo para adicionar estilos personalizados ao seu aplicativo.

6. **Compilar o projeto:**
   - Para criar a versão de produção do seu aplicativo, execute:
     ```bash
     npm run build
     ```
   - Isso gerará uma pasta `dist` que contém os arquivos estáticos do seu projeto e que podem rodar no navegador.

**Extra: Publique seu site no Netlify**