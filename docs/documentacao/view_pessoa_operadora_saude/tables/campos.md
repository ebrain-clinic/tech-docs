| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do vínculo de operadora | Obrigatório |
| data_registro | timestamp | Data de registro do vínculo |  |
| pessoa_unique_cod | varchar | Código único da pessoa relacionada ao vínculo | Obrigatório |
| operadora_saude_unique_cod | varchar | Código único da operadora de saúde | Obrigatório se `nome_operadora` nulo |
| numero | varchar | Número da carteirinha |  |
| validade | date | Data de validade da carteirinha |  |
| nome_operadora | varchar | Nome da operadora de saúde | Obrigatório se `operadora_saude_unique_cod` nulo |
| detalhes | varchar | Detalhes adicionais do vínculo com a operadora |  |
| plano_unique_cod | varchar | Código único do plano de saúde |  |
| nome_plano | varchar | Nome do plano de saúde |  |
