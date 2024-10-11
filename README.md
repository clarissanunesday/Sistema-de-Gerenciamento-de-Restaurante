# Sistema de Gerenciamento de Restaurante

Este projeto implementa um sistema básico de gerenciamento de pedidos para um restaurante, abrangendo clientes, mesas, pedidos e itens de pedidos. O sistema é projetado para armazenar e organizar informações dos clientes, mesas disponíveis no restaurante, pedidos realizados e os itens consumidos em cada pedido.

## Funcionalidades

- **Gestão de Clientes**: Armazena informações dos clientes, incluindo nome, telefone e e-mail.
- **Gestão de Mesas**: Armazena o número da mesa e sua capacidade de assentos.
- **Gestão de Pedidos**: Permite registrar pedidos, associando-os a um cliente e a uma mesa.
- **Gestão de Itens de Pedido**: Registra os itens consumidos em cada pedido, como descrição, quantidade e preço unitário.
  
## Estrutura do Banco de Dados

### Tabelas:

- **Clientes**:
  - `id_cliente`: Identificador único do cliente.
  - `nome`: Nome do cliente.
  - `telefone`: Telefone do cliente.
  - `email`: E-mail do cliente.

- **Mesas**:
  - `id_mesa`: Identificador único da mesa.
  - `numero_mesa`: Número da mesa.
  - `capacidade`: Número de assentos disponíveis na mesa.

- **Pedidos**:
  - `id_pedido`: Identificador único do pedido.
  - `id_cliente`: Identificador do cliente associado ao pedido.
  - `id_mesa`: Identificador da mesa associada ao pedido.
  - `data_pedido`: Data e hora em que o pedido foi realizado.
  - `total`: Valor total do pedido.

- **Itens_Pedido**:
  - `id_item`: Identificador único do item de pedido.
  - `id_pedido`: Identificador do pedido ao qual o item pertence.
  - `descricao_item`: Descrição do item consumido.
  - `quantidade`: Quantidade do item consumido.
  - `preco_unitario`: Preço unitário do item.

## Consultas Disponíveis

1. **Listar todos os clientes**:
   - Exibe todas as informações dos clientes cadastrados no sistema.

2. **Listar todas as mesas**:
   - Exibe a lista de mesas e suas respectivas capacidades.

3. **Listar todos os pedidos**:
   - Exibe os pedidos realizados, incluindo data, cliente e mesa.

4. **Exibir os itens de um pedido específico e calcular o subtotal**:
   - Exibe a descrição dos itens de um pedido, quantidade, preço unitário e subtotal (quantidade x preço).

5. **Calcular o total de um pedido específico**:
   - Exibe o valor total do pedido.

## Como Usar

1. **Criar o Banco de Dados**:
   Execute o script SQL fornecido para criar o banco de dados e as tabelas necessárias.

2. **Inserir Dados**:
   Use o script SQL para inserir os dados iniciais, incluindo clientes, mesas, pedidos e itens de pedidos.

3. **Consultar e Atualizar Dados**:
   Utilize as consultas SQL para visualizar e atualizar informações conforme necessário.

4. **Deletar Dados**:
   Execute comandos SQL para remover registros de pedidos e itens relacionados.

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

## Requisitos

- MySQL ou outro sistema de gerenciamento de banco de dados compatível com SQL.
- Editor SQL para execução de consultas e scripts.
