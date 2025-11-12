| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do serviço                       |     Obrigatório            |
| nome               | varchar | Nome do serviço                                      |   Obrigatório              |
| data_inicio          | timestamp     | Data do ínicio deste serviço                   |   Obrigatório              |
| data_importacao    | timestamp     | Data que ocorreu a importação     |                 |
| data_fim | Timestamp     |   Data que o serviço parou de ser realizado        |                 |
| agendavel            | boolean |   Indica se é agendavel      |                 |
| agendavel_via_app               | boolean | Indica se é agendável via app                 |                 |
| gratuito     | boolean   | Indica se é um serviço gratuito                                  |                 |
| atende_particular     | boolean   | Indica se aceita atendimento particular                                  |                 |
| atende_convenio     | boolean   | Indica se aceita convênio médico                                 |                 |
| especialidade_id     | varchar   | ID(s) da(s) especialidade(s) do serviço, separados por vírgula. Ex: "18" ou "1,3,18" (ver [especialidades](documentacao/view_especialidade/))                                 |                 |
| valor_particular     |  decimal(10, 2)   | Valor do serviço particular                           |                 |
| modelo_unique_cods     | varchar   | Código(s) único(s) do(s) modelo(s) de equipamento associado(s) ao serviço, separados por vírgula. Ex: "ABC123" ou "ABC123,DEF456"                           |                 |
| prontuario_indicacao_produto     | boolean   | Indica se o serviço permite associação com produtos                           |                 |
