| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do grupo de contas | Obrigatório |
| clinica_unique_cod | varchar | Código único da clínica associada ao grupo de contas | Obrigatório caso haja mais de uma clínica |
| caixa_padrao_unique_cod | varchar | Código único do livro caixa padrão associado ao grupo de contas |  |
| nome | varchar | Nome do grupo de contas |  |
| padrao | boolean | Indica se o grupo de contas é o padrão |  |
| data_inicio | date | Data de início de vigência do grupo de contas |  |
