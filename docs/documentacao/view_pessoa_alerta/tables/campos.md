| Campo                       | Tipo      | Descrição                                                                  | Restrição       |
|-----------------------------|-----------|----------------------------------------------------------------------------|-----------------|
| unique_cod                 | varchar     | Código único sem repetição do alerta                     |     Obrigatório            |
| pessoa_unique_cod | varchar     |   Código do paciente                         |      Obrigatório           |
| data_registro          | timestamp     | Data do registro                        |   Obrigatório              |
| data_exclusao    | timestamp     | Data de exclusão               |                 |
| descricao               | varchar | Descrição do alerta                                   |   Obrigatório              |
| concluido          | boolean     | Indica se foi concluído                  |   Obrigatório              |
| inclusor_unique_cod | varchar |  Código do usuário que incluiu o alerta         |      Obrigatório           |
