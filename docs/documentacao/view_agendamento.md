# Agendamento
<p align="justify"> 
Neste documento, estão descritos os campos necessários para importar os dados de agendamento no sistema Ebrain. A tabela de descrição dos campos abrange as principais informações do evento agendado, bem como os serviços relacionados ao agendamento, independentemente do número de serviços envolvidos. Além disso, também é registrado se o agendamento foi efetivamente realizado.
 </p>

## Descrição dos campos

| Campo                        | Tipo       | Descrição                                                                                         | Restrição   |
|------------------------------|------------|---------------------------------------------------------------------------------------------------|-------------|
| externo_cod                  | varchar    | Chave primária da pessoa                                                                          | Obrigatório | 
| descricao                    |   varchar | Descrição do agendamento                                                                                                  |             |
| data_registro                | timestamp  | Data de registro  |  Obrigatório     | 
| hora_inicio                  |   timestamp  | Hora do ínicio marcada                                                                                                |             |
| hora_fim                     |    timestamp  | Hora do fim marcada  | |
| data_chegada                 | timestamp       |  Data da chegada do paciente  |             |
| hora_inicio_efetivo          | timestamp  |  Hora que efetivamente ocorre o atendimento                                                                                               |             |
| hora_fim_efetivo             | timestamp   | Hora que efetivamente acaba o atendimento| |
| observacoes                  |  varchar   | Referente à quaisquer observações                                                                                                  |             |
| motivo_nao_atendimento       |  varchar          |  Motivo do não atendimento                                                                                                 |             |
| nao_atendido                 |  boolean          |  Indica que não houve o atendimento                                                                                                 |             |
| encaixe                      |  boolean          |  Indica se é um encaixe                                                                                                 |             |
| remoto                       |  boolean          |  Indica se é um atendimento remoto                                                                                                  |             |
| particular                   |  boolean          |  Indica se é um atendimento particular                                                                                                  |             |
| dia_todo                     |  boolean          |  Indica se é o dia todo                                                                                                  |             |
| pessoa_externo_cod           |  varchar          |  Código do paciente   |      |
| operadora_saude_externo_cod  |  varchar          | Código da operadora de saúde                                                                                                   |             |
| profissional_externo_cod     | varchar           |  Código do profissional responsável                                                                                                 |             |
| serv_1_servico_externo_cod   |  varchar          | Código do serviço relacionado                                                                                                  |             |
| serv_1_observacao            |  varchar          |  Quaisquer observações sobre o serviço                                                                                                 |             |
| serv_1_realizado             |  boolean          |  Indica se o serviço foi realizado                                                                                                 |             |
| serv_1_quantidade            | numeric(21,2)            |  Quantidade realizada do serviço                                                                                                 |             |
| serv_2_servico_externo_cod   |  varchar          | Código do serviço relacionado                                                                                                  |             |
| serv_2_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv_2_realizado             |  boolean          | Indica se o serviço foi realizado                                                                                                  |             |
| serv_2_quantidade            | numeric(21,2)            | Quantidade realizada do serviço                                                                                                  |             |
| serv_3_servico_externo_cod   | varchar          |   Código do serviço relacionado                                                                                                |             |
| serv_3_observacao            | varchar           | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv_3_realizado             |  boolean          |  Indica se o serviço foi realizado                                                                                                 |             |
| serv_3_quantidade            | numeric(21,2)            |  Quantidade realizada do serviço                                                                                                 |             |
| serv_4_servico_externo_cod   |  varchar          |  Código do serviço relacionado                                                                                                 |             |
| serv_4_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv_4_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv_4_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço                                                                                                 |             |
| serv_5_servico_externo_cod   |  varchar         |  Código do serviço relacionado                                                                                                 |             |
| serv_5_observacao            | varchar           | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv_5_realizado             |  boolean          | Indica se o serviço foi realizado                                                                                                  |             |
| serv_5_quantidade            |  numeric(21,2)           |  Quantidade realizada do serviço                                                                                                 |             |
