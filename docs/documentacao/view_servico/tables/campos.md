| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do serviço                       |     Obrigatório            |
| nome               | varchar | Nome do serviço                                      |   Obrigatório              |
| data_inicio          | timestamp     | Data do ínicio deste serviço                   |   Obrigatório              |
| data_importacao    | timestamp     | Data que ocorreu a importação     |                 |
| data_fim | timestamp     | Data que o serviço parou de ser realizado        |                 |
| evo_admin_id | int | ID do serviço no sistema EVO (interno) |  |
| agendavel            | boolean |   Indica se é agendavel      |                 |
| agendavel_via_app               | boolean | Indica se é agendável via app                 |                 |
| gratuito     | boolean   | Indica se é um serviço gratuito                                  |                 |
| atende_particular     | boolean   | Indica se aceita atendimento particular                                  |                 |
| atende_convenio     | boolean   | Indica se aceita convênio médico                                 |                 |
| aplicavel_todas_especialidades | boolean | Indica se o serviço é aplicável a todas as especialidades |                 |
| valor_particular     |  decimal(10, 2)   | Valor do serviço particular                           |                 |
| especialidade_id_aplicaveis | varchar | IDs de especialidades aplicáveis ao serviço, separados por vírgula. Ex: "18" ou "1,3,18" (ver [especialidades](documentacao/view_especialidade/)) |                 |
| categoria | varchar | Categoria do serviço (ex.: "Procedimentos") |                 |
| modelo_unique_cods     | varchar   | Código(s) único(s) do(s) modelo(s) de equipamento associado(s) ao serviço, separados por vírgula. Ex: "ABC123" ou "ABC123,DEF456" (ver [equipamentos](documentacao/view_equipamento/))                           |                 |
| diagnostico_associacao_automatica | boolean | Indica se o serviço associa diagnóstico automaticamente |                 |
| minutos_duracao_padrao | int | Duração padrão do serviço em minutos |                 |
| prontuario_indicacao_produto | varchar | Indica se o serviço permite associação com produtos |                 |
