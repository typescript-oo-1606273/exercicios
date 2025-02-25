# Exercício: Sistema de Gerenciamento de Pedidos

## Objetivo
Desenvolver um sistema simples para gerenciar os pedidos de uma loja utilizando conceitos básicos de TypeScript, tais como enums, type aliases, tipos primitivos e funções.

## Cenário
Uma loja precisa organizar os pedidos dos clientes. Cada pedido possui um status representado por um enum e contém informações como:
- **ID:** Identificador único do pedido.
- **Nome do Cliente:** Nome do cliente que realizou o pedido.
- **Itens:** Lista dos itens comprados, onde cada item tem um nome e um valor.
- **Status:** Etapa atual do pedido, que pode ser "Pendente", "Processando", "Enviado" ou "Entregue". O status inicial deve ser sempre "Pendente".

## Instruções

1. **Definir os Status com um Enum**
   - Crie um `enum` chamado `StatusPedido` com os seguintes valores:
     - `PENDENTE`
     - `PROCESSANDO`
     - `ENVIADO`
     - `ENTREGUE`
   - Utilize string literals para definir os valores, garantindo que somente esses estados sejam aceitos.

2. **Criar os Tipos dos Dados utilizando `type`**
   - **Tipo `Item`:**
     - Propriedades:
       - `nome`: string
       - `valor`: number
   - **Tipo `Pedido`:**
     - Propriedades:
       - `id`: number
       - `nomeCliente`: string
       - `itens`: array de `Item`
       - `status`: do tipo `StatusPedido` (inicia sempre como `PENDENTE`)

3. **Função para Calcular o Valor Total do Pedido**
   - Implemente uma função que receba um objeto do tipo `Pedido` e retorne a soma dos valores de todos os itens do pedido.

4. **Função para Atualizar o Status do Pedido**
   - Crie uma função que receba um objeto do tipo `Pedido` e um novo status (do tipo `StatusPedido`), atualize o status do pedido e retorne o pedido atualizado.

5. **Função para Exibir as Informações do Pedido**
   - Desenvolva uma função que formate e retorne uma string contendo os detalhes do pedido, incluindo:
     - Nome do cliente.
     - Lista dos itens (nome e valor).
     - Valor total (calculado anteriormente).
     - Status atual do pedido.

6. **Testar o Sistema**
   - Crie um pedido de exemplo com alguns itens.
   - Utilize as funções criadas para:
     - Calcular o valor total.
     - Atualizar o status (por exemplo, de `PENDENTE` para `PROCESSANDO`, depois para `ENVIADO` e, por fim, para `ENTREGUE`).
     - Exibir os detalhes do pedido a cada etapa.
