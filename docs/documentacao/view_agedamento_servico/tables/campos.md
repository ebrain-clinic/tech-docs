| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do serviço do agendamento | Obrigatório |
| ordem | integer | Ordem na aplicação |  |
| agendamento_unique_cod | varchar | Código único do agendamento ao qual o serviço está associado | Obrigatório |
| profissional_unique_cod | varchar | Código do profissional responsável pelo serviço |  |
| quantidade | numeric | Quantidade do serviço realizado | Obrigatório |
| servico_unique_cod | varchar | Código único do serviço | Obrigatório |
| item_pedido_unique_cod | varchar | Código do item do pedido associado ao serviço |  |
| observacao | varchar | Observações sobre o serviço |  |
| realizado | boolean | Indica se o serviço foi realizado | Obrigatório |
| pago | boolean | Indica se o serviço foi pago |  |
| data_registro | timestamp | Data de registro do serviço | Obrigatório |
| data_exclusao | timestamp | Data de exclusão do serviço |  |
| inclusor_unique_cod | varchar | Código do usuário que fez a inclusão do registro |  |
| pessoa_unique_cod | varchar | Código do paciente |  |
| agenda_especialidade_cod | int | ID da especialidade da agenda (ver [especialidades](documentacao/view_especialidade/)) |  |
