| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do contato | Obrigatório |
| data_registro | timestamp | Data de registro do contato |  |
| pessoa_unique_cod | varchar | Código único da pessoa relacionada ao contato | Obrigatório |
| descricao | varchar | Descrição do contato. Use `celular`, `fixo` ou o e-mail | Obrigatório |
| telefone_ddd | int | DDD do telefone (quando aplicável) |  |
| num_ddi | int | DDI do telefone (quando aplicável) |  |
| telefone_numero | int | Número do telefone (quando aplicável) |  |
| telefone_numero_completo | varchar | Número completo do telefone |  |
| preferido | boolean | Indica se o contato é preferido | Obrigatório |
| receber_propagandas | boolean | Indica se o contato recebe propagandas | Obrigatório |
| receber_confirmacoes | boolean | Indica se o contato recebe confirmações | Obrigatório |
| possui_whatsapp | boolean | Indica se o contato possui WhatsApp |  |
