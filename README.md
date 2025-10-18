
# 🧩 Normalização de Dados — Sistema de Pedidos

## 🧠 Antes da Normalização
Inicialmente, todas as informações estavam concentradas em uma única tabela chamada **“pedidos”**, que reunia dados de **clientes, produtos e pedidos** no mesmo espaço.

### Problemas encontrados:
- **Redundância:** o mesmo cliente e produto apareciam repetidamente em várias linhas.  
- **Manutenção difícil:** qualquer atualização exigia mudanças em diversos registros.  
- **Inconsistências:** dados de um mesmo cliente poderiam divergir entre linhas.  
- **Dependências incorretas:** campos de clientes e produtos dependiam de atributos que não eram diretamente relacionados.

![](https://github.com/francisgust/normalizacao-de-dados/blob/main/tabelapedidos.png)
