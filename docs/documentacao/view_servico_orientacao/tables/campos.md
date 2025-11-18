| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição da orientação de serviço | Obrigatório |
| servico_unique_cod | varchar | Código único do serviço ao qual esta orientação está vinculada (ver [Serviços](documentacao/view_servico/)) | Obrigatório |
| titulo | varchar | Título da orientação | Obrigatório |
| descricao | text | Texto completo da orientação a ser enviada ao paciente. Pode conter emojis e variáveis como @paciente | Obrigatório |
| tipo_evento_servico_orientacao | varchar | Tipo de evento que dispara o envio da orientação (ex.: "HORA_ATENDIMENTO", "HORA_AGENDADA", "HORA_REGISTRO") | Obrigatório |
| horas_decorridas | int | Número de horas decorridas em relação ao evento para envio da orientação. Valores positivos indicam envio após o evento, valores negativos indicam envio antes do evento | |
| dias_decorridos | int | Número de dias decorridos em relação ao evento para envio da orientação. Valores positivos indicam envio após o evento, valores negativos indicam envio antes do evento | |
| envio_automatico_app | boolean | Indica se a orientação deve ser enviada automaticamente via aplicativo | Obrigatório |
| data_registro | timestamp | Data e hora de registro da orientação | Obrigatório |
| data_exclusao | timestamp | Data e hora de exclusão lógica da orientação (soft delete) | |
| nome_servico | varchar | Nome do serviço (campo auxiliar para visualização) | |
| especialidade_id_aplicaveis | varchar | IDs de especialidades aplicáveis a esta orientação, separados por vírgula. Ex: "18" ou "1,3,18" (ver [especialidades](documentacao/view_especialidade/)) | |
