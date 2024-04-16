# Agendamento

<p align="justify"> 
Descreve a estrutura de dados de agendamento. A tabela de descrição dos campos abrange as informações do evento agendado, bem como os serviços relacionados ao agendamento, independentemente do número de serviços envolvidos. Além disso, também é registrado se o agendamento foi efetivamente realizado.
 </p>

> Nome do arquivo de importação: `import_agendamento.csv`

## Descrição dos campos

| Campo                        | Tipo       | Descrição                                                                                         | Restrição   |
|------------------------------|------------|---------------------------------------------------------------------------------------------------|-------------|
| unique_cod                  | varchar    | Código único sem repetição do agendamento                                                                          | Obrigatório | 
| descricao                    |   varchar | Descrição do agendamento, como o nome da pessoa, caso ainda não esteja cadastrada                                                                                                  |             |
| data_registro                | timestamp  | Data de registro  |  Obrigatório     | 
| hora_inicio                  |   timestamp  | Hora do ínicio marcada. Como é um agendamento, pode ser uma data no futuro, para agendamento vindouros, ou no passado, caso já tenha transcorrido o tempo do agendamento                                                                                                 |             |
| hora_fim                     |    timestamp  | Hora do fim marcada. Ver `hora_inicio`  | |
| data_chegada                 | timestamp       |  Data da chegada do paciente na clínica |             |
| hora_inicio_efetivo          | timestamp  |  Hora que efetivamente ocorreu o atendimento. Será sempre uma data do passado                                                                                                |  Obrigatório caso o evento tenha de fato acontecido           |
| hora_fim_efetivo             | timestamp   | Hora que efetivamente acaba o atendimento. Será sempre uma data do passado | Obrigatório caso o evento tenha de fato acontecido |
| observacoes                  |  varchar   | Referente à quaisquer observações                                                                                                  |             |
| motivo_nao_atendimento       |  varchar          |  Motivo do não atendimento                                                                                                 |             |
| nao_atendido                 |  boolean          |  Indica que não houve o atendimento                                                                                                 |             |
| encaixe                      |  boolean          |  Indica se é um encaixe                                                                                                 |             |
| remoto                       |  boolean          |  Indica se é um atendimento remoto                                                                                                  |             |
| particular                   |  boolean          |  Indica se é um atendimento particular                                                                                                  |             |
| dia_todo                     |  boolean          |  Indica se é o dia todo                                                                                                  |             |
| pessoa_unique_cod           |  varchar          |  Código do paciente   |      |
| operadora_saude_externo_cod  |  varchar          | Código da operadora de saúde                                                                                                   |             |
| profissional_unique_cod     | varchar           |  Código do profissional responsável                                                                                                 |             |
| usuario_registro_unique_cod     | varchar           |  Código do usuário responsável pelo registro                                                                                                 |             |
| serv1_servico_unique_cod   |  varchar          | Código do serviço relacionado                                                                                                  |             |
| serv1_observacao            |  varchar          |  Quaisquer observações sobre o serviço                                                                                                 |             |
| serv1_realizado             |  boolean          |  Indica se o serviço foi realizado                                                                                                 |             |
| serv1_quantidade            | numeric(21,2)            |  Quantidade realizada do serviço                                                                                                 |             |
| serv2_servico_unique_cod   |  varchar          | Código do serviço relacionado                                                                                                  |             |
| serv2_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv2_realizado             |  boolean          | Indica se o serviço foi realizado                                                                                                  |             |
| serv2_quantidade            | numeric(21,2)            | Quantidade realizada do serviço                                                                                                  |             |
| serv3_servico_unique_cod   | varchar          |   Código do serviço relacionado                                                                                                |             |
| serv3_observacao            | varchar           | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv3_realizado             |  boolean          |  Indica se o serviço foi realizado                                                                                                 |             |
| serv3_quantidade            | numeric(21,2)            |  Quantidade realizada do serviço                                                                                                 |             |
| serv4_servico_unique_cod   |  varchar          |  Código do serviço relacionado                                                                                                 |             |
| serv4_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv4_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv4_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço                                                                                                 |             |
| serv5_servico_unique_cod   |  varchar         |  Código do serviço relacionado                                                                                                 |             |
| serv5_observacao            | varchar           | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv5_realizado             |  boolean          | Indica se o serviço foi realizado                                                                                                  |             |
| serv5_quantidade            |  numeric(21,2)           |  Quantidade realizada do serviço                                                                                                 |             |
| serv6_servico_unique_cod   |  varchar          |  Código do serviço relacionado                                                                                                 |             |
| serv6_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv6_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv6_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço  
| serv7_servico_unique_cod   |  varchar          |  Código do serviço relacionado                                                                                                 |             |
| serv7_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv7_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv7_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço                                                                                                 |             |
| serv8_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv8_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv8_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço                                                                                                 |             |
| serv9_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv9_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv9_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço         
| serv10_observacao            |  varchar          | Quaisquer observações sobre o serviço                                                                                                   |             |
| serv10_realizado             |   boolean         |   Indica se o serviço foi realizado                                                                                                |             |
| serv10_quantidade            | numeric(21,2)  |  Quantidade realizada do serviço                                                                                                 |             |        
| agenda_especialidade_cod            |  varchar          | Especialidade da agenda em que serão importados os agendamentos                                                                                                   |             |
| nome_agenda_importacao             |   varchar         |   Nome da agenda em que serão importados os agendamentos                                                                                                |             |
| agenda_coletiva            | boolean  |  Indica se a agenda é coletiva                                                                                                 |             |                                                                 


## Arquivo
<p align="justify">Arquivo de exemplo:</p>

[Clique aqui para baixar o arquivo csv de exemplo](arquivos_exemplos/import_agendamento.csv ':ignore')
