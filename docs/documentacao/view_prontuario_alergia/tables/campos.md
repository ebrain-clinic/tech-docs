| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição da alergia                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| nome          | varchar     | Nome da alergia                        |   Obrigatório              |
| observacao    |  varchar    | Observações à respeito da alergia               |                 |
| relevante_prescricoes               | boolean | Se possui prescrições relevantes                                  |   Obrigatório              |
| data_registro          | timestamp     |   Data do registro                |   Obrigatório              |
| data_fim |timestamp | Data fim da alergia | |
| prontuario_especialidade_cod | int | Código da especialidade do prontuário (se houver) |  |
| inclusor_unique_cod            | varchar |  Código do usuário que registrou as alergias         |      Obrigatório           |
