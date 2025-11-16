| Campo                             | Tipo      | Descrição                                                                 | Restrição   |
|-----------------------------------|-----------|--------------------------------------------------------------------------|---------------|
| unique_cod                        | varchar   | Código único sem repetição para cada linha de prescrição.                 | Obrigatório |
| data_informada                    | timestamp | Data informada no documento.                                             |             |
| data_exclusao                     | timestamp | Data da exclusão do documento.                                           |             |
| pessoa_unique_cod                 | varchar   | Código do paciente vinculado ao documento.                                | Obrigatório |
| profissional_unique_cod           | varchar   | Código do profissional que fez o documento.                              | Obrigatório |
| prontuario_unique_cod             | varchar   | Código do prontuário que contém o documento.                             | Obrigatório |
| documento_texto                   | varchar   | Prescrição textual que contém o conteúdo do relatório médico.             | Obrigatório |
| inclusor_unique_cod               | varchar   | Código do usuário que incluiu o documento.                                |  |
| prontuario_especialidade_cod      | int       | Código da especialidade do prontuário (se houver)                         |  |
