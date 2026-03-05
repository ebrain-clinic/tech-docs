| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do meio de transação | Obrigatório |
| nome | varchar | Nome do meio de transação |  |
| ordem | int | Ordem de exibição do meio de transação |  |
| data_fim | date | Data de encerramento do meio de transação |  |
| tipo_conta | varchar | Tipo de conta ao qual o meio de transação se aplica | Valores esperados no importador atual: `RECEBIMENTO`, `PAGAMENTO` |
| complemento | varchar | Informações complementares do meio de transação |  |
| data_inicio | date | Data de início de vigência do meio de transação |  |
| max_parcelas | int | Quantidade máxima de parcelas permitidas |  |
| min_parcelas | int | Quantidade mínima de parcelas permitidas |  |
| freq_parcelas | int | Frequência entre parcelas |  |
| dias_tipo_contagem | varchar | Tipo de contagem dos dias do parcelamento | Valores válidos quando informado: `UTIL`, `CORRIDO` |
| valor_min_parcela | numeric | Valor mínimo por parcela |  |
| caixa_unique_cod | varchar | Código único do livro caixa associado ao meio de transação |  |
| tipo_lancamento | varchar | Forma de lançamento no caixa para transações parceladas | Valores válidos quando informado: `UNICO`, `PARCELADO` |
| plano_conta_taxa_unique_cod | varchar | Código único do plano de contas utilizado para registrar taxa do meio de transação |  |
| pessoa_juridica_pagamento_taxa_unique_cod | varchar | Código único da pessoa jurídica que recebe o pagamento da taxa |  |
