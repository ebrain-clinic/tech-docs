| Campo                          | Tipo      | Descrição                                                            | Restrição   |
|--------------------------------|-----------|----------------------------------------------------------------------|-------------|
| unique_cod                     | varchar   | Código único do registro de consumo                                  | Obrigatório |
| ordem                          | integer   | Ordem do consumo                                                     |             |
| item_pedido_unique_cod         | varchar   | Código único do item do pedido consumido                             | Obrigatório |
| quantidade_consumida           | numeric   | Quantidade consumida do item (deve ser maior que 0)                  | Obrigatório |
| data_registro                  | timestamp | Data e hora de registro do consumo                                   | Obrigatório |
| data_consumo                   | timestamp | Data e hora em que o serviço foi efetivamente consumido              |             |
| profissional_unique_cod        | varchar   | Código único do profissional que realizou o serviço                  | Obrigatório |
| inclusor_unique_cod            | varchar   | Código único do usuário que registrou o consumo                      |             |
| usuario_pedido_unique_cod      | varchar   | Código único do usuário responsável pela venda                       |             |
| agendamento_servico_unique_cod | varchar   | Código único do agendamento de serviço relacionado ao consumo        |             |
| servico_unique_cod             | varchar   | Código único do serviço consumido                                    |             |
