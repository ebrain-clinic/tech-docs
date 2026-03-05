| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição da conta | Obrigatório |
| conta_grupo_unique_cod | varchar | Código único do grupo de contas associado |  |
| plano_conta_unique_cod | varchar | Código único do plano de contas associado |  |
| pessoa_unique_cod | varchar | Código único da pessoa associada à conta |  |
| pedido_unique_cod | varchar | Código único do pedido associado à conta |  |
| data_registro | timestamp | Data de registro da conta |  |
| tipo_conta | varchar | Tipo da conta | Valores esperados no importador atual: `PAGAMENTO`, `RECEBIMENTO` |
| descricao | varchar | Descrição da conta |  |
| data_vencimento | date | Data de vencimento da conta |  |
| valor_inicial | numeric | Valor inicial da conta |  |
| valor_recebido_pago | numeric | Valor efetivamente recebido ou pago na conta |  |
| total_parcelas | int | Quantidade total de parcelas associadas à conta |  |
