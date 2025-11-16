| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do antecedente                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| descricao          | varchar     | Descrição dos antecedentes                        |   Obrigatório              |
| privado               | boolean | Se é privado                                  |                 |
| data_registro          | timestamp     |   Data do registro                |   Obrigatório              |
| prontuario_especialidade_cod | int | Código da especialidade do prontuário (se houver) |  |
| inclusor_unique_cod            | varchar |  Código do usuário que registrou os antecedentes         |      Obrigatório           |
