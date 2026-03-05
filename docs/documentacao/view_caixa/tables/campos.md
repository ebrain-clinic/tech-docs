| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do livro caixa | Obrigatório |
| nome | varchar | Nome do livro caixa |  |
| data_fim | timestamp | Data de encerramento do livro caixa |  |
| data_inicio | timestamp | Data de início do livro caixa |  |
| tipo_pessoa | varchar | Tipo de pessoa associada ao livro caixa (`PF`: Pessoa Física, `PJ`: Pessoa Jurídica) | Valores válidos quando informado: `PF`, `PJ` |
| nome_reduzido | varchar | Nome reduzido do livro caixa | Máximo de 15 caracteres |
| conta_bancaria | boolean | Indica se o livro caixa representa uma conta bancária |  |
| percentual_reducao_comissoes | numeric | Percentual de redução de comissões aplicado ao livro caixa |  |
| clinica_unique_cod | varchar | Código único da clínica associada ao livro caixa | Obrigatório caso haja mais de uma clínica |
