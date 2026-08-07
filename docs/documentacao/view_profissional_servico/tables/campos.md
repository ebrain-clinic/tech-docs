| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do vínculo entre profissional e serviço | Obrigatório |
| data_registro | timestamp | Data e hora de registro do vínculo |  |
| minutos_duracao_padrao | int | Duração padrão do serviço para o profissional, em minutos |  |
| valor_particular | numeric | Valor particular do serviço para o profissional |  |
| atende_particular | bool | Indica se o profissional atende o serviço de forma particular |  |
| atende_convenio | bool | Indica se o profissional atende o serviço por convênio |  |
| profissional_unique_cod | varchar | Código único do profissional associado ao serviço | Obrigatório |
| servico_unique_cod | varchar | Código único do serviço associado ao profissional | Obrigatório |
