| Campo                        | Tipo      | Descrição                                             | Restrição  |
| ---------------------------- | --------- | ------------------------------------------------------- | ------------ |
| unique_cod                   | varchar   | Código único do pedido                                | Obrigatório |
| orcamento_unique_cod         | varchar   | Código único do orçamento original associado         |              |
| data_pedido                  | date      | Data do pedido                                          |              |
| data_registro                | timestamp | Data e hora de registro do pedido                       | Obrigatório |
| data_exclusao                | timestamp | Data e hora de exclusão do pedido                      |              |
| valor_total_pedido           | numeric   | Valor total do pedido                                   |              |
| total_pago                   | numeric   | Valor total pago                                        |              |
| pacote                       | boolean   | Indica se o pedido é parte de um pacote                |              |
| cortesia                     | boolean   | Indica se o pedido é uma cortesia                      |              |
| pessoa_unique_cod            | varchar   | Código único do paciente associado ao pedido          |              |
| profissional_unique_cod      | varchar   | Código único do profissional responsável pelo pedido | Obrigatório |
| usuario_pedido_unique_cod    | varchar   | Código único do usuário responsável pela venda      |              |
| inclusor_unique_cod          | varchar   | Código único do usuário que incluiu o pedido         |              |
| clinica_unique_cod           | varchar   | Código único da clínica associada                    |              |
| operadora_saude_unique_cod   | varchar   | Código único da operadora de saúde                   |              |
| operadora_codigo_autorizacao | varchar   | Código de autorização da operadora de saúde         |              |