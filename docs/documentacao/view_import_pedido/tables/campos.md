| Campo                        | Tipo        | Descrição                                                                           | Restrição       |
|------------------------------|-------------|-------------------------------------------------------------------------------------|-----------------|
| unique_cod                   | varchar     | Código único do pedido                                           | Obrigatório     |
| orcamento_unique_cod         | varchar     | Código único do orçamento original associado                                       | Obrigatório     |
| data_pedido                        | varchar     | data do pedido                                                             |                 |
| data_registro               | timestamp | Data e hora de registro do pedido                                       |   Obrigatório              |
| data_exclusao               | timestamp | Data e hora de exclusão do pedido                        |                 |
| valor_total_pedido        | numeric     | Valor total do pedido do orçamento                                                           |                 |
| total_pago        | numeric     | Valor total pago                                                                                 |                 |
| pacote                       | varchar     | Indica se o orçamento é parte de um pacote                                          |                 |
| cortesia                     | varchar     | Indica se o orçamento é uma cortesia                                                |                 |
| pessoa_unique_cod            | varchar     | Código único do paciente associado ao pedido                                     | Obrigatório     |
| profissional_unique_cod      | varchar     | Código único do profissional responsável pelo pedido                             | Obrigatório     |
| usuario_pedido_unique_cod    | varchar     | Código único do usuario responsavel pela venda                                       | Obrigatório     |
| inclusor_unique_cod          | varchar     | Código único do usuario que incluiu o pedido                                      | Obrigatório     |
| clinica_unique_cod           | varchar     | Código único da clínica associada                                                   |                 |
| operadora_saude_unique_cod   | varchar     | Código único da operadora de saúde                                                  |                 |
| operadora_codigo_autorizacao | varchar     | Código de autorização da operadora de saúde                                         |                 |
