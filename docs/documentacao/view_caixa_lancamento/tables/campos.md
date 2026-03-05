| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do lançamento de caixa | Obrigatório |
| inclusor_unique_cod | varchar | Código único do usuário responsável pelo lançamento |  |
| meio_transacao_unique_cod | varchar | Código único do meio de transação utilizado no lançamento |  |
| data_pagamento | timestamp | Data e hora do pagamento ou recebimento |  |
| descricao | varchar | Descrição do lançamento de caixa |  |
| valor | numeric | Valor do lançamento de caixa |  |
| caixa_unique_cod | varchar | Código único do livro caixa associado ao lançamento |  |
| plano_conta_unique_cod | varchar | Código único do plano de contas associado ao lançamento |  |
| tipo_lancamento | varchar | Tipo do lançamento de caixa | Valores esperados no importador atual: `PAGAMENTO`, `RECEBIMENTO` |
