
# 🧩 Normalização de Dados — Sistema de Pedidos

## 🧠 Antes da Normalização
Inicialmente, todas as informações estavam concentradas em uma única tabela chamada **“pedidos”**, que reunia dados de **clientes, produtos e pedidos** no mesmo espaço.

### Problemas encontrados:
- **Redundância:** o mesmo cliente e produto apareciam repetidamente em várias linhas.  
- **Manutenção difícil:** qualquer atualização exigia mudanças em diversos registros.  
- **Inconsistências:** dados de um mesmo cliente poderiam divergir entre linhas.  
- **Dependências incorretas:** campos de clientes e produtos dependiam de atributos que não eram diretamente relacionados.

![](https://github.com/francisgust/normalizacao-de-dados/blob/main/tabelapedidos.png)

 ## ✅ Depois da Normalização
O banco de dados foi reorganizado em **múltiplas tabelas**, cada uma com uma função específica.  
Essa separação eliminou redundâncias, simplificou atualizações e melhorou o desempenho geral.

### Estrutura após o processo:
- **Clientes:** contém apenas informações básicas (nome, ID, etc).  
- **Contatos:** armazena os meios de contato de cada cliente.  
- **Endereços:** guarda os endereços completos associados a cada cliente.  
- **Produtos:** registra informações únicas de cada item (descrição, categoria, preço).  
- **Pedidos:** armazena os dados principais da compra (data, valor, forma de pagamento, cliente).  
- **Itens do Pedido:** liga produtos aos pedidos, mostrando o que foi comprado e em que quantidade.

![](https://github.com/francisgust/normalizacao-de-dados/blob/main/tabelanormalizada.png)
