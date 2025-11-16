| Campo | Tipo | Descrição | Restrição |
| --- | --- | --- | --- |
| unique_cod | varchar | Código único sem repetição do agendamento | Obrigatório |
| descricao | varchar | Descrição do agendamento, como o nome da pessoa, caso ainda não esteja cadastrada |  |
| descricao_status_personalizado | varchar | Possíveis status de agendamento da clínica, que são específicos a ela |  |
| registro_automatico_trigger | varchar | São triggers que relacionamos com a descricao_status_personalizado para compor a tipo_evento_agendado_status. Ver valores possíveis abaixo |  |
| data_registro | timestamp | Data de registro | Obrigatório |
| hora_inicio | timestamp | Hora do ínicio marcada. Como é um agendamento, pode ser uma data no futuro, para agendamento vindouros, ou no passado, caso já tenha transcorrido o tempo do agendamento |  |
| hora_fim | timestamp | Hora do fim marcada. Ver `hora_inicio` |  |
| data_chegada | timestamp | Data da chegada do paciente na clínica |  |
| data_confirmacao | timestamp | Data de confirmação da consulta do paciente na clínica |  |
| hora_inicio_efetivo | timestamp | Hora que efetivamente ocorreu o atendimento. Será sempre uma data do passado | Obrigatório se o evento tenha sido realizado |
| hora_fim_efetivo | timestamp | Hora que efetivamente acaba o atendimento. Será sempre uma data do passado | Obrigatório se o evento tenha sido realizado |
| observacoes | varchar | Referente à quaisquer observações |  |
| motivo_nao_atendimento | varchar | Motivo do não atendimento |  |
| dominio_motivo_cancelamento | varchar | Tipo de motivo de cancelamento. Ver valores possíveis abaixo |  |
| nao_atendido | boolean | Indica que não houve o atendimento |  |
| encaixe | boolean | Indica se é um encaixe |  |
| remoto | boolean | Indica se é um atendimento remoto |  |
| particular | boolean | Indica se é um atendimento particular |  |
| dia_todo | boolean | Indica se é o dia todo |  |
| pessoa_unique_cod | varchar | Código do paciente |  |
| operadora_saude_unique_cod | varchar | Código da operadora de saúde |  |
| profissional_unique_cod | varchar | Código do profissional responsável |  |
| inclusor_unique_cod | varchar | Código do usuário responsável pelo registro |  |
| agenda_especialidade_cod | int | ID da especialidade da agenda em que serão importados os agendamentos (ver [especialidades](documentacao/view_especialidade/)) |  |
| nome_agenda_importacao | varchar | Nome da agenda em que serão importados os agendamentos |  |
| agenda_coletiva | boolean | Indica se a agenda é coletiva |  |
| clinica_unique_cod | varchar | Código único da clínica |  |
| bloqueio | varchar | Indica se o agendamento é ou não um bloqueio. Valores possíveis: IMPORTAR_COMO_BLOQUEIO, IMPORTAR_COMO_AGENDAMENTO, NAO_IMPORTAR, NULL |  |
