| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do histórico da parcela | Obrigatório |
| conta_unique_cod | varchar | Código único da conta associada ao histórico |  |
| conta_parcela_unique_cod | varchar | Código único da parcela associada ao histórico |  |
| meio_transacao_unique_cod | varchar | Código único do meio de transação associado ao histórico |  |
| inclusor_unique_cod | varchar | Código único do usuário responsável pelo lançamento |  |
| caixa_lancamento_unique_cod | varchar | Código único do lançamento de caixa associado ao histórico |  |
| data_registro | timestamp | Data de registro do histórico |  |
| data_lancamento | timestamp | Data e hora do lançamento do histórico |  |
| tipo_lancamento | varchar | Tipo de lançamento do histórico | Valores válidos quando informado: `REGISTRO`, `RECEBIMENTO`, `PAGAMENTO`, `CANCELAMENTO`, `EXCLUSAO`, `ALTERACAO_VALOR` |
| valor | numeric | Valor do lançamento do histórico | Obrigatório |
| valor_restante | numeric | Valor restante da parcela após o lançamento |  |
| descricao | varchar | Descrição do histórico |  |
| meio_transacao_parcelas | int | Quantidade total de parcelas do meio de transação |  |
| meio_transacao_parcela_atual | int | Número da parcela atual dentro do meio de transação |  |
