| Campo                        | Tipo        | Descrição                                                                           | Restrição       |
|------------------------------|-------------|-------------------------------------------------------------------------------------|-----------------|
| unique_cod                   | varchar     | Código único do orçamento ou procedimento                                           | Obrigatório     |
| data_orcamento               | timestamp   | Data de criação do orçamento                                                        | Obrigatório     |
| data_registro                | timestamp   | Data e hora de registro do orçamento                                                | Obrigatório     |
| data_validade_orcamento      | timestamp   | Data de vencimento do orçamento                                                     | Obrigatório     |
| data_exclusao                | timestamp   | Data de exclusão do orçamento                                                       |                 |
| orcamento_concluido          | boolean     | Indica se o orçamento está concluído                                                |                 |
| negocio_fechado              | boolean     | Indica se o negócio foi fechado                                                             |                 |
| observacao                   | varchar     | Observações gerais do orçamento                                                     |                 |
| instrucoes_realizacao        | varchar     | Instruções para realização do orçamento                                             |                 |
| valor_total_orcamento        | numeric     | Valor total do orçamento                                                           |                 |
| pessoa_unique_cod            | varchar     | Código único do paciente associado ao orçamento                                     | Obrigatório     |
| profissional_unique_cod      | varchar     | Código único do profissional responsável pelo orçamento                             | Obrigatório     |
| usuario_pedido_unique_cod    | varchar     | Código único do usuario responsavel pela venda                                       | Obrigatório     |
| inclusor_unique_cod          | varchar     | Código único do usuario que incluiu o orçamento                                      | Obrigatório     |
| clinica_unique_cod           | varchar     | Código único da clínica associada                                                   |                 |
