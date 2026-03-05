| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do plano de contas | Obrigatório |
| plano_conta_pai_unique_cod | varchar | Código único do plano de contas superior, para composição da hierarquia |  |
| codigo | varchar | Código hierárquico do plano de contas. Exemplo: `1`, `1.1`, `2.3.4` |  |
| descricao | varchar | Descrição do plano de contas |  |
| data_registro | timestamp | Data de registro do plano de contas |  |
